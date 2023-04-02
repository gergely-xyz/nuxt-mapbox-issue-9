<template>
  <div>
    <NuxtLink to="/other"> Click here to go to another page </NuxtLink>
    <MapboxMap
      map-id="map2"
      style="top: 80px"
      :options="{
        style: 'mapbox://styles/mapbox/streets-v12', // style URL
        center: [100.0, 0.0], // starting position [lng, lat]
        zoom: 3, // starting zoom
      }"
    >
      <MapboxFullscreenControl :options="{}" />
      <MapboxNavigationControl :options="{}" />
    </MapboxMap>
  </div>
</template>

<script setup></script>
