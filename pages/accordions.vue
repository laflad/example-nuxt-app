<template>
    <div>
      <main class="main text-center">
        <h1 class="heading">Pets make everything better!</h1>
        <p>Explore benefits of the type of pets below.</p>
  
        <!-- Accordion loop -->
        <!-- added a little bit of styling for interest -->
        <div class="accordion m-5 w-50 mx-auto" id="accordionExample">
          <div class="accordion-item addspace" v-for="item in items"
                :key="item.id">
            <button class="accordion-button collapsed awesome" type="button" data-bs-toggle="collapse" :data-bs-target="'#collapse'+item.id" aria-expanded="false" aria-controls="collapseOne">
                {{ item.title }}
            </button>
            <div :id="'collapse'+item.id" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
              <div class="accordion-body">
                <ul v-for="(detail, id) in item.details" :key="id" class="list-group list-group-flush list-style">
                  <li>{{ detail }}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </main>
    </div>
</template>

<script>
export default {
data() {
    return {
    items: [ 
        { 
        id: 1,
        title: 'Why cats are the best!',
        details: [
            'They clean themselves.',
            'They catch bugs and rodents.',
            'They dont bark.',
            'They are low maintence',
            'You can leave them alone for a full day',
            'You can actually teach them trick! Ask Winston!',
        ]
        },
        {
        id: 2,
        title: 'Why dogs are also awesome!',
        details: [
            'They instantly love you without needing to earn it.',
            'They are fun to do outdoor adventures with.',
            'They guard your house.',
            'They encourage you to move around.',
            'The are social magnets.',
            'They help brighten our mood and reduce anxiety.',
        ]
        },
        {
        id: 3,
        title: 'Want even lower maintence?',
        details: [ 
            'Get a plant!',
        ]
        },
    ]
    }
},
name: 'AccordionPage',
props: {
    msg: String
},

}
</script>

<style lang="scss">
.addspace {
  padding-bottom: .5rem;
}

.awesome {
  width: 500px;
  text-align: left;
  border: none;
  border-radius: 5px;
  padding: 1rem;
  background: linear-gradient(0deg, rgba(0,80,103,1) 0%, rgba(0,104,135,1) 35%, rgba(16,127,161,1) 100%); 
  color: white;
}

.list-style {
  text-align: left !important;
  padding-left: 4rem;
  list-style: none;
}

.heading {
  text-align: center;
  font-size: 2rem;
  color: #555;
  margin: 2rem auto;
}
</style>