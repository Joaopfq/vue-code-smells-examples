<script lang="ts">
export default {
  data() {
    return {
      user: null as { name: string } | null, // Pode ser nulo
    };
  },
  methods: {
    getUserName() {
      return this.user!.name; // Assume que `user` nunca será nulo
    },
  },
};
</script>
