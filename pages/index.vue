<script setup lang="ts">
  definePageMeta({
    // layout: 'default',
    // name: 'index',
    // alias: 'index',
    title: 'Home',
    description: 'Sip, Savor, and Spark Ideas at The AI Cafe!',
    navOrder: 1,
    type: 'primary',
    icon: 'i-mdi-home',
  })
</script>
<template>
  <div>
    <section class="h-[500px] relative">
      <v-carousel class="absolute w-screen">
        <v-carousel-item
          v-for="(item, index) in 4"
          :key="index"
          :alt="`hero${index + 1}`"
          :src="`images/hero${index + 1}.jpg`"
          cover
        >
        </v-carousel-item>
      </v-carousel>
    </section>
    <div class="container mx-auto p-10">
      <section class="specials py-8">
        <div>
          <h2 class="text-2xl font-bold text-center mb-4">Today's Specials</h2>
          <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
            <div class="card">
              <v-img
                src="https://images.unsplash.com/photo-1493770348161-369560ae357d?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE3fHxmb29kfGVufDB8fHx8MTY5NzI5MTk3Mnww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                alt="Food Image"
                class="rounded-lg"
              ></v-img>
              <div class="card-content">
                <h3 class="text-lg font-bold">Delicious Food</h3>
                <p class="text-sm">Try our mouthwatering dishes</p>
              </div>
            </div>
            <div class="card">
              <v-img
                alt="Drinks Image"
                src="https://images.unsplash.com/photo-1485872299829-c673f5194813?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDF8fGRyaW5rc3xlbnwwfHx8fDE2OTcyOTQwMDJ8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                class="rounded-lg"
              ></v-img>
              <div class="card-content">
                <h3 class="text-lg font-bold">Refreshing Drinks</h3>
                <p class="text-sm">
                  Quench your thirst with our refreshing drinks
                </p>
              </div>
            </div>
            <div class="card">
              <v-img
                src="https://images.unsplash.com/photo-1541167760496-1628856ab772?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDZ8fGNvZmZlZXxlbnwwfHx8fDE2OTcyOTIwNDF8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                alt="Coffee Image"
                class="card-image rounded-lg"
              ></v-img>
              <div class="card-content">
                <h3 class="text-lg font-bold">Premium Coffee</h3>
                <p class="text-sm">Discover our rich and flavorful coffee</p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="testimonials py-8">
        <div>
          <h2 class="text-2xl font-bold text-center mb-4">Testimonials</h2>
          <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
            <div class="card text-center">
              <v-avatar
                alt="Avatar - John Doe"
                class="card-image rounded-full w-20 h-20 mx-auto"
              >
                <v-img
                  src="https://images.unsplash.com/photo-1544725176-7c40e5a71c5e?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wyMDkyMnwwfDF8c2VhcmNofDEyfHxhdmF0YXJ8ZW58MHx8fHwxNjk3MzQxNjcxfDA&ixlib=rb-4.0.3&q=80&w=200"
                  alt="John Doe"
                  cover
                />
              </v-avatar>
              <div class="card-content">
                <h3 class="text-lg font-bold">John Doe</h3>
                <p class="text-sm">
                  "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Aenean euismod ligula nec commodo vestibulum. Sed venenatis mi
                  at ex gravida, sed volutpat augue bibendum."
                </p>
              </div>
            </div>
            <div class="card text-center">
              <v-avatar
                alt="Avatar - Jane Smith"
                class="card-image rounded-full w-20 h-20 mx-auto"
              >
                <v-img
                  src="https://images.unsplash.com/photo-1566492031773-4f4e44671857?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE1fHxhdmF0YXJ8ZW58MHx8fHwxNjk3MzQxNjcxfDA&ixlib=rb-4.0.3&q=80&w=200"
                  alt="Jane Smith"
                  cover
                />
              </v-avatar>
              <div class="card-content">
                <h3 class="text-lg font-bold">Jane Smith</h3>
                <p class="text-sm">
                  "Fusce fermentum, nisl ac convallis bibendum, lectus erat
                  eleifend enim, ut efficitur ante turpis sed nulla. Maecenas
                  congue purus eget scelerisque vestibulum."
                </p>
              </div>
            </div>
            <div class="card text-center">
              <v-avatar
                alt="Avatar - David Johnson"
                class="card-image rounded-full w-20 h-20 mx-auto"
              >
                <v-img
                  src="https://images.unsplash.com/photo-1543610892-0b1f7e6d8ac1?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE2fHxhdmF0YXJ8ZW58MHx8fHwxNjk3MzQxNjcxfDA&ixlib=rb-4.0.3&q=80&w=200"
                  alt="David Johnson"
                  cover
                />
              </v-avatar>
              <div class="card-content">
                <h3 class="text-lg font-bold">David Johnson</h3>
                <p class="text-sm">
                  "Vestibulum volutpat ante eu velit vulputate, et maximus
                  lectus facilisis. Etiam efficitur est et ante commodo, vitae
                  consequat orci egestas."
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="get-in-touch py-8">
        <div>
          <h2 class="text-2xl font-bold text-center mb-4">Get In Touch</h2>
          <div class="grid grid-cols-1 sm:grid-cols-2 gap-8">
            <div class="sm:col-span-1">
              <v-text-field label="Name" outlined></v-text-field>
            </div>
            <div class="sm:col-span-1">
              <v-text-field label="Mobile Number" outlined></v-text-field>
            </div>
            <div class="sm:col-span-2">
              <v-text-field label="Email Address" outlined></v-text-field>
            </div>
            <div class="flex justify-center sm:col-span-2">
              <v-btn color="primary" outlined>Submit</v-btn>
            </div>
          </div>
        </div>
      </section>
      <section class="">
        <v-row>
          <v-col cols="12" sm="6" md="4">
            <v-card>
              <v-img
                src="https://images.unsplash.com/photo-1557142046-c704a3adf364?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDd8fGNhZmUlMjBmb29kfGVufDB8fHx8MTY5NzI5MjA0Mnww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                alt="Eggs Benedict"
              />
              <v-card-text>
                <h3 class="text-lg font-bold">Eggs Benedict</h3>
                <p>
                  Classic breakfast dish with poached eggs, crispy bacon, and
                  creamy hollandaise sauce served on an English muffin.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4">
            <v-card>
              <v-img
                src="https://images.unsplash.com/photo-1613697193450-23f766dbaa73?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDEzfHxjYWZlJTIwZm9vZHxlbnwwfHx8fDE2OTcyOTIwNDJ8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                alt="Avocado Toast"
              />
              <v-card-text>
                <h3 class="text-lg font-bold">Avocado Toast</h3>
                <p>
                  Smashed avocado on toasted whole wheat bread, topped with
                  cherry tomatoes, feta cheese, and a drizzle of balsamic glaze.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4">
            <v-card>
              <v-img
                src="https://images.unsplash.com/photo-1610632380989-680fe40816c6?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE2fHxjb2ZmZWV8ZW58MHx8fHwxNjk3MjkyMDQxfDA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
                alt="Cappuccino"
              />
              <v-card-text>
                <h3 class="text-lg font-bold">Cappuccino</h3>
                <p>
                  A classic Italian espresso-based beverage, topped with steamed
                  milk and a sprinkle of cocoa powder.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </section>
    </div>
  </div>
</template>
<style scoped></style>
