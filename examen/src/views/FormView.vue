<template>
    <div>
        <b-breadcrumb>
      <b-breadcrumb-item href="#home">
        <b-icon icon="house-fill" scale="1.25" shift-v="1.25" aria-hidden="true"></b-icon>
        Home
      </b-breadcrumb-item>
      <b-breadcrumb-item active>Form</b-breadcrumb-item>
    </b-breadcrumb>
        <h1>Ingrese sus datos</h1>
        <form id="app" @submit="checkForm">
            <p>
                <label for="name">Nombre</label>
                <input id="name" v-model="name" type="text" name="name">
            </p>
            <p>
                <label for="age">Edad</label>
                <input id="age" v-model="age" type="number" name="age" min="0">
            </p>
            <p>
                <label for="career">Carrera</label>
                <select id="career" v-model="career" name="career">
                    <option>Desarrollo y gestion de software</option>
                    <option>Admnistración empresarial</option>
                    <option>Diseño de modas</option>
                    <option>Diseño digital</option>
                    <option>Mecatronica</option>
                </select>
            </p>
            <p>
                <button type="submit">Enviar</button>
            </p>
        </form>
    </div>
</template> 

<script>
</script>
<style></style>