<template>
<div class="layout-padding image">
    <div class="row justify-center">
     <q-card class="card-login">
     <q-card-section class="q-ma-sm card" style="width: 350px;">
      <div class="text-center" style="color: #0D0D0D;">INICIAR SESIÓN <q-icon  name="verified_user"/></div>
      <q-car-section>
        <q-form>
         <q-input
            icon name="verified_user"
            v-model="username"
            label="Usuario*"
            hint="Nombre de usuario o correo"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'ingrese un valor permitido']"
             />
              <q-input
            v-model="password"
            label="Contraseña*"
            hint="Ingrese la contraseña registrada"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'ingrese un valor permitido']"
             />
                <q-card-actions>
                <q-btn label="Ingresar" type="submit" color="green"/>
                <q-btn label="Calcelar" type="reset" color="grey" flat class="q-ml-sm" />
                </q-card-actions>
        </q-form>
      </q-car-section>
     </q-card-section>
    </q-card>
   </div>
  </div>
</template>

<script>
export default {
  // name: 'PageName',
}
</script>
