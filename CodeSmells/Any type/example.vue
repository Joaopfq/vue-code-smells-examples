<script lang="ts">
export default {
  data() {
    return {
      user: {} as any, // O tipo `any` permite qualquer valor
    };
  },
  methods: {
    setUser(newUser: any) { // Parâmetro do tipo `any`
      this.user = newUser;
    },
    printUser() {
      console.log(this.user.name); // Nenhuma garantia de que `name` existe
    },
  },
};
</script>
