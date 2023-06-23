<template>
  <div>
    <br />
    <br />
    <br />
    <!--  -->
    <v-row>
      <v-col md="1" lg="2" xl="2" sm="12"></v-col>
      <v-col md="10" lg="8" xl="8"  sm="12">
        <v-row>
          <v-col md="6" sm="12">
            <div style="font-size: 28px" class="pt-5">
              SABA IP WAS FOUNDED IN 1926 AT A TIME WHEN THE FIELD OF
              INTELLECTUAL PROPERTY LAW, IN THE MIDDLE EAST, WAS STILL IN ITS
              INFANCY.
            </div>
          </v-col>
          <v-col md="6" sm="12">
            <lite-youtube
              videoid="D7RqEAolEzo"
              params="wmode=transparent&amp;autoplay=1"
              title="YouTube video player 1"
              style="
                background-image: url('https://i.ytimg.com/vi/D7RqEAolEzo/hqdefault.jpg');
              "
              class="lyt-activated"
              ><button type="button" class="lty-playbtn">
                <span class="lyt-visually-hidden">Play</span></button
              ><iframe
                width="560"
                height="315"
                title="Play"
                allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen=""
                src="https://www.youtube-nocookie.com/embed/D7RqEAolEzo?wmode=transparent&amp;autoplay=1&amp;autoplay=1"
              ></iframe
            ></lite-youtube>
          </v-col>
        </v-row>
        <!--  -->
        <br />
        <br />
        <br />
        <br />
        <br />
        <v-card class="card-border pt-5 pb-5">
          <v-card-item>
            <v-row class="text-center">
              <v-col md="4" sm="12" class="vl">
                <v-card-title class="pt-5">WHO WE ARE </v-card-title>

                <div class="pt-5 pb-5">
                  Saba & Co. Intellectual Property (Saba IP) was founded in
                  1926, at a time when the field of Intellectual Property Law,
                  in the Middle East, was still in its infancy.
                </div>
                <div class="pt-5 pb-5">
                  <v-btn
                    variant="tonal"
                    class="uppercase button-color"
                    size="large"
                  >
                    read more
                  </v-btn>
                </div>
              </v-col>
              <!-- <div class="vl"></div> -->

              <v-col md="4" sm="12" class="vl">
                <v-card-title class="pt-5">WHAT WE DO </v-card-title>

                <div class="pt-5">
                  <div class="my-3">IP Rights Counseling</div>
                  <hr />

                  <div class="my-3">Enforcement & Litigation</div>
                  <hr />

                  <div class="my-3">Related IP Services</div>
                  <hr />
                </div>
              </v-col>

              <v-col md="4" sm="12" class="vl">
                <v-card-title class="pt-5">WHERE WE WORK </v-card-title>

                <div class="pt-5">
                  Operating through an extensive network of branch and
                  representative offices across the Middle East, Africa and
                  neighboring regions, we enjoy the reputation of a leading
                  service provider.
                </div>
                <div class="pt-5 pb-5">
                  <v-btn
                    variant="tonal"
                    class="uppercase button-color"
                    size="large"
                  >
                    office locations
                  </v-btn>
                </div>
              </v-col>
            </v-row>
          </v-card-item>
        </v-card>
        <!--  -->
      </v-col>
     <v-col md="1" lg="2" xl="2" sm="12"></v-col>
    </v-row>

    <!--  -->
    <br />
    <br />
    <br />
    <br />
    <div style="background-color: #1a3c59; color: white">
      <v-row class="pt-5">
        <v-col md="1" lg="2" xl="2" sm="12"></v-col>
        <v-col md="8" xs="12">
          <v-sheet class="d-flex mb-6 bg-transparent">
            <v-sheet
              class="ma-2 pa-2 me-auto bg-transparent"
              style="font-size: 29px"
              >IF YOU STAND OUT, YOU FIT IN!
            </v-sheet>
            <v-sheet class="ma-2 pa-2 bg-transparent">
              <div>
                <v-btn
                  variant="tonal"
                  class="uppercase"
                  size="x-large"
                  style="background-color: white; color: black"
                >
                  careers
                </v-btn>
              </div>
            </v-sheet>
          </v-sheet>
        </v-col>
       <v-col md="1" lg="2" xl="2" sm="12"></v-col>
      </v-row>
    </div>

    <!-- LATEST NEWS -->
    <br />
    <br />
    <br />
    <br />
    <div class="pt-5 pb-5">
      <v-row>
        <v-col md="1" lg="2" xl="2" sm="12"></v-col>
        <v-col md="10" lg="8" sm="12">
          <div
            class="text-center pb-5 font-weight-bold"
            style="font-size: 30px"
          >
            LATEST NEWS
          </div>
          <!--  -->
          <div></div>
          <!--  -->
          <br />
          <v-row>
            <v-col md="4" sm="12" v-for="item in items" :key="item">
              <v-hover v-slot="{ isHovering, props }">
                <v-card
                  class="mx-auto"
                  color=""
                  max-width="600"
                  v-bind="props"
                  style="height: 400px"
                >
                  <v-img :aspect-ratio="16 / 9" cover :src="item.img">
                    <v-expand-transition>
                      <div
                        v-if="isHovering"
                        class="d-flex transition-fast-in-fast-out v-card--reveal text-center"
                        style="
                          height: 100%;
                          background-color: #1a3c59;
                          color: white;
                        "
                      >
                        {{ item.hoverText }}
                      </div>
                    </v-expand-transition>
                  </v-img>

                  <v-card-item>
                    <div>{{ item.title }}</div>

                    <v-card-subtitle class="pt-3">
                      {{ item.date }}
                    </v-card-subtitle>
                  </v-card-item>
                </v-card>
              </v-hover>
            </v-col>
          </v-row>
        </v-col>
       <v-col md="1" lg="2" xl="2" xs="12"></v-col>
      </v-row>
    </div>
    <!-- check all industry news -->
    <div class="pt-5 pb-3 text-center pb-5">
      <v-btn variant="tonal" class="uppercase button-color" size="large">
        check all industry news
      </v-btn>
    </div>
    <br />
    <!-- WE OPERATE ACROSS THE MIDDLE EAST AND AFRICA -->
    <v-row style="background-color: #1a3c59; color: white">
      <v-col md="2" sm="12"></v-col>
      <v-col md="8" sm="12">
        <v-row>
          <v-col md="7" xs="12" class="mx-sm-5">
            <h2 class="my-5 text-cente">
              WE OPERATE ACROSS THE MIDDLE EAST AND AFRICA
            </h2>
            <center>
              <hr class="w-25" />
            </center>
            <h3 class="pt-5" style="font-weight: 400">
              We provide a wide range of legal and paralegal services in the
              Middle East, Africa, and their neighboring regions through an
              extensive network of branch and representative offices. Our Head
              Office in Lebanon provides IP services in countries in the rest of
              the world through our widely established network of associate
              firms.
            </h3>
          </v-col>
          <v-col md="5" xs="12">
            <v-img
              src="https://www.sabaip.com/wp-content/uploads/2021/07/map-400x194.png"
              style="width: 60%"
            />
            <!--  -->
            <div class="d-flex flex-row mb-6">
              <v-sheet class="ma-2 pa-2">
                <v-btn variant="plain">stay connected</v-btn>
              </v-sheet>
              <v-sheet class="ma-2 pa-2">
                <v-btn variant="plain">view map</v-btn>
              </v-sheet>
            </div>
          </v-col>
        </v-row>
      </v-col>
      <v-col md="2" xs="12"></v-col>
    </v-row>

    <!-- FAQS -->
    <v-row class="pt-5">
      <v-col md="3" sm="12"></v-col>
      <v-col md="6" sm="12" class="mx-sm-5">
        <h1 class="text-center" style="font-weight: 400">FAQS</h1>
        <br />
        <br />
        <v-expansion-panels class="">
          <v-expansion-panel
            class="my-2"
            v-for="expan in expansion"
            :key="expan"
            :title="expan.title"
            :text="expan.content"
          ></v-expansion-panel>
        </v-expansion-panels>

        <div class="text-center pt-5">
          <v-btn variant="tonal" class="uppercase button-color" size="large">
            still curious
          </v-btn>
        </div>
      </v-col>
      <v-col md="3" xs="12"></v-col>
    </v-row>
  </div>
</template>

<script lang="ts" setup>
import HelloWorld from "@/components/HelloWorld.vue";
const items = [
  {
    img: "/public/one.webp",
    hoverText: "TMO in Libya Resumes Operations",

    title: "TMO in Libya Resumes Operations",
    date: "June 20th, 2023",
  },
  {
    img: "/public/two.jpg",
    hoverText:
      "Oman Implements Progressive Fee Adjustments to Foster Intellectual Property Growth",
    title:
      "Oman Implements Progressive Fee Adjustments to Foster Intellectual Property Growth",
    date: "June 1st, 2023",
  },
  {
    img: "/public/three.jpg",
    hoverText:
      "USPTO and OMPIC Collaborate to Accelerate Patent Processing with PPH Program",
    title:
      "USPTO and OMPIC Collaborate to Accelerate Patent Processing with PPH Program",
    date: "April 20th, 2023",
  },
];
const expansion = [
  {
    title:
      "What factors should brand owners consider when choosing a trademark in Arabic?",
    content:
      "When the trademark in question can be transliterated in different phonetic renditions, a vast scope of inconsistencies may come as a result of this  Careful thought and consideration must therefore be taken from the outset to select the most accurate and appropriate transliteration and to ensure that this version is consistently used",
  },
  {
    title:
      " What are the advantages of registering the Arabic rendition of a Latin trademark?",
    content:
      " When it comes to the treatment of trademarks in a multi-lingual context, trademark laws of Arab countries are traditionally designed to avoid conflicts between marks across different languages, and to provide specifically for the protection of the transliteration of marks. Accordingly, the registration of a trademark in its Latin (original) script in any Arab country should, in general, provide protection against the registration of another confusingly similar transliteration liable to create public confusion. However, while the transliteration of the mark is protected, likelihood of confusion is easier to prove when comparing marks in the same language. Having said that, registering trademarks in transliterated Arabic script, in addition to their original format, is advisable considering that most Arab countries are in principal governed by civil law – that is, the concept of first to file carries considerable weight. While some countries may offer a limited number of common law rights, registration is highly recommended and can be used as a basis on which to sue an infringer.",
  },
  {
    title:
      "To what extent are trademark laws harmonized in the Middle East countries?",
    content: "",
  },

  {
    title: "What are the rules for using the ™ or ® symbol?",
    content:
      "In principal, the ™ symbol may be used when trademark rights are claimed in relation to a mark that has not been registered at the Trademark Office of a particular jurisdiction, meaning that, the use of the ™ symbol does not mean a legally enforceable    trademark. The registration symbol ®, however, does carry legal   weight. It should only be used when the mark is registered with  the Trademark Office of a particular jurisdiction. Using the symbol  ® illegitimately may be treated as fraudulent marking in most  of the countries in our region.   Marking is not compulsory in the Middle East and North Africa. However, using any of those symbols  on a trademark is advisable because it will give notice to the public about the owners’ rights",
  },
];
</script>
<style></style>
