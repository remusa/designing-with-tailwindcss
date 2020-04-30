<template>
  <div class="bg-white border rounded-lg overflow-hidden">
    <div class="p-6">
      <img :src="property.imageUrl" :alt="property.imageAlt" />
      <h4>{{ property.title }}</h4>
      <div>{{ property.beds }} beds &bull; {{ property.baths }} baths</div>
      <div>{{ property.formattedPrice }} / week</div>
      <div>
        {{ property.rating }}/5 (based on {{ property.reviewCount }} reviews)
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['property'],
}
</script>

<style></style>
