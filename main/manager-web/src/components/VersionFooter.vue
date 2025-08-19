<template>
  <div class="copyright">
    <div class="footer-content">
      <span>© {{ currentYear }} xiaolang beta 1.0.0</span>

    </div>
  </div>
</template>

<script>
export default {
  name: 'VersionFooter',
  computed: {
    currentYear() {
      return new Date().getFullYear()
    }
  }
}
</script>

<style scoped>
.copyright {
  padding: 10px 0;
}

.footer-content {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
  color: #666;
}
</style>