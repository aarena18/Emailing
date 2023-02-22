<template>
    <div>
      <h1>Formulaire de commentaires</h1>
      <form @submit.prevent="submitForm">
        <label for="nom">Nom:</label>
        <input type="text" id="nom" v-model="nom" required>
        <label for="prenom">Prénom:</label>
        <input type="text" id="prenom" v-model="prenom" required>
        <label for="commentaire">Commentaire:</label>
        <textarea id="commentaire" v-model="commentaire"></textarea>
        <button type="submit">Envoyer</button>
      </form>
    </div>
</template>
  
<script>
  export default {
    data() {
      return {
        nom: '',
        prenom: '',
        commentaire: '',
      }
    },
    methods: {
      submitForm() {
        // soumettre le formulaire
        console.log(this.nom, this.prenom, this.commentaire)
      }
    },
  }
</script>

<style scoped>
    form {
    display: flex;
    flex-direction: column;
    width: 400px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    }

    label {
    font-size: 1.2rem;
    margin-top: 10px;
    }

    input,
    textarea {
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    }

    input:focus,
    textarea:focus {
    border-color: #0078e7;
    outline: none;
    }

    button[type="submit"] {
    background-color: #0078e7;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    font-size: 1.2rem;
    cursor: pointer;
    }

    button[type="submit"]:hover {
    background-color: #005cbf;
    }
</style>
  