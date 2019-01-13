<template>
    <div id="app">
        <Home msg="Hello world!" />
        <SystemInfo name="VTR Development" tags="{'DEV','VTR'}" url="http://vtr.local/" />
        <SystemInfo name="VTR System Testing" server="SVRAPPS4" tags="{'SIT','VTR'}" url="http://vtrtest.elections.nsw.gov.au/" />
        <SystemInfo name="VTR User Acceptance Testing" server="SVRAPPS2" tags="{'UAT','VTR'}" url="http://vtrstaging.elections.nsw.gov.au/" />
        <SystemInfo name="VTR Production" server="Azure Web App" tags="{'PROD','VTR'}" url="http://vtrprod.elections.nsw.gov.au/" />
    </div>
</template>

<script>
    import Home from './components/Home.vue';
    import SystemInfo from './components/SystemInfo.vue';

    export default {
        name: 'app',
        components: {
            Home,
            SystemInfo
        }
    };
</script>

<style>
</style>
