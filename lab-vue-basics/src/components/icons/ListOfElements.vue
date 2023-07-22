<script setup>
import { ref } from 'vue';

const animes = ref([
    {
        id: 1,
        title: 'Naruto',
        description: 'Naruto is a Japanese manga series written and illustrated by Masashi Kishimoto. It tells the story of Naruto Uzumaki, a young ninja who seeks recognition from his peers and dreams of becoming the Hokage, the leader of his village.',
        content: 'The story begins during Naruto adolescence, around the age of twelve. Orphan dunce and great prankster, he does all possible stupidity to get noticed. His dream: to become the best Hokage in order to be recognized by the inhabitants of his village. Indeed, the nine-tailed fox demon sealed within him has fueled the fear and contempt of the other villagers, who, over time, no longer differentiate between Kyūbi and Naruto.',
        
    },
    {
        id: 2,
        title: 'Hunter X Hunter',
        description: 'Is a Japanese manga series written and drawn by Yoshihiro Togashi . It is pre-published sinceMarch 1998in publisher Shūeisha Weekly Shōnen Jump , and is compiled into thirty-seven volumes.',
        content: 'Gon Freecss is a 12-year-old boy who dreams of becoming a hunter . Hunters are elite citizens authorized to do almost anything they want on simple presentation of their license: they can thus acquire for free any object for sale on the funds of the association, requisition any vehicle, accommodation and tool for their work and are de facto authorized to practice all the professions in the world, being able as well to become bounty hunters, chefs, archaeologists, zoologists, vigilantes or consultants in various fields.', 
        
    },
    {
        id: 3,
        title: 'One Piece',
        description: 'One Piece is a shōnen manga series created by Eiichirō Oda. It has been pre-published since July 22, 1997 in the weekly magazine Weekly Shōnen Jump, then grouped in tankōbon with Shūeisha editions since December 24, 1997. 106 volumes are marketed in Japan in July 2023.',
        content: 'The story follows the adventures of Monkey D. Luffy , a boy whose body acquired the properties of rubber after he inadvertently ate a Devil Fruit. Along with his pirate crew , called the Straw Hat Crew , Luffy explores the Grand Line in search of the ultimate treasure known as "One Piece" in order to become the next Pirate King.',
    },
])
</script>

<template>
    <div>
        <h2 class="top-three"> Favorite Anime</h2>
        <ul class="anime">
            <li class="anime-list" v-for="anime in animes" :key="anime.id">
                <h3>{{ anime.title }}</h3>
                <p>{{ anime.description }}</p>
                <p>{{ anime.content }}</p>
            </li>
        </ul>
    </div>
</template>


<style>
.top-three {
    font-family: Arial, Helvetica, sans-serif;
    background-color: rgb(187, 86, 176);
    padding: 10px;
    margin-top: 50px;
    margin-bottom: 50px;
}
.anime {
    list-style-type: none;
    padding: 0;
    text-align: center;
}
.anime-list {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    background-color: rgb(237, 224, 205);
    margin-bottom: 20px;
    border: 1px solid #000;
    padding: 10px;
}
</style>