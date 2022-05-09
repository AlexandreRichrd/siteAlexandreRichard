<template>
  <div :class="$style['formulaire']">
    <div :class="$style['NomPrenom']">
      <div :class="$style['nom']">
        <label for="nom">Nom*</label>
        <input id="nom" type="text"/>
      </div>
      <div :class="$style['prenom']">
        <label for="nom">Prénom*</label>
        <input id="nom" type="prenom"/>
      </div>
    </div>
    <div :class="$style['email']">
      <label for="email">E-mail*</label>
      <input id="email" type="email" name="email" />
    </div>
    <div :class="$style['tel']">
      <label for="tel">Téléphone</label>
      <input id="tel" type="phone" name="tel" pattern="^((\+\d{1,3}(-| )?\(?\d\)?(-| )?\d{1,5})|(\(?\d{2,6}\)?))(-| )?(\d{3,4})(-| )?(\d{4})(( x| ext)\d{1,5}){0,1}$"/>
    </div>
    <div :class="$style['description']">
      <label for="description">Description du projet*</label>
      <textarea />
    </div>
    <div :class="$style['checkConditionsUtilisation']">
      <input id="conditions" type="checkbox" name="conditions">
      <label for="conditions">J’accepte que les informations saisies soient utilisées dans le cadre de la soumission du projet et des futurs échanges.</label>
    </div>
    <a>Envoyer</a>
  </div>
</template>

<script>

  export default {
    
  }
</script>

<style module>
.formulaire{
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
}

.NomPrenom{
  display: flex;
  justify-content: center;
  gap: 3rem;
}

.nom{
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.nom input{
  width: 10rem;
  height: 1.8rem;
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
}

.prenom{
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.prenom input{
  width: 10rem;
  height: 1.8rem;
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
}

.email{
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.email input{
  width: 23rem;
  height: 1.8rem;
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
}

.tel{
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.tel input{
  width: 23rem;
  height: 1.8rem;
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
}

.description{
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

textarea{
  width: 23rem;
  height: 7rem;
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
  resize: none;
}

.checkConditionsUtilisation{
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.checkConditionsUtilisation input{
  border: 0;
  border-radius: 8px;
  background-color: var(--background-color);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
  height: 1.4rem;
  width: 1.4rem;
  cursor: pointer;
}

.checkConditionsUtilisation label{
  width: 21rem;
  font-size: 0.6rem;
  color: #848484;
  text-align: justify;
  cursor: pointer;
}

.formulaire a{
  background-color: var(--main-color);
  width: 23rem;
  height: 2.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #FFF;
  cursor: pointer;
}

label{
  text-align: left;
  font-weight: 400;
  padding-left: 0.1rem;
}
</style>