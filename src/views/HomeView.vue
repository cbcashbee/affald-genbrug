<script setup>
import Affaldshierarki from '../components/Affaldshierarki.vue';
import Forebyggelse from '../components/Forebyggelse.vue';
import Genbrug from '../components/Genbrug.vue';
import Genanvendelse from '../components/Genanvendelse.vue';
import Energi from '../components/Energi.vue';
import Deponi from '../components/Deponi.vue';
</script>

<template>
    <div id="intro">
        <p id="bread">Forside | Affald & Genbrug | Fakta om affald | Affaldshierarkiet</p>
        <Affaldshierarki />
    </div>
    <Forebyggelse />
    <div class="box-full" id="box-gen">
        <Genbrug /> 
    </div>
    <Genanvendelse />
    <div class="box-full" id="box-ene">
        <Energi />
    </div>
    <Deponi />
    <div class="space"/>
    <footer />
</template>
