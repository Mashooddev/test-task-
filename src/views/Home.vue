
<template>
	<div class="w-full ">
		<Header/>
	<section class="grid grid-cols-1 md:grid-cols-2  lg:grid-cols-4 gap-4 px-5 py-3">
		<div v-for="({image,name,profileImage,title,views}) in singleCardData">
			<SingleCard
			 :image="image"
			 :profileImage="profileImage"
			 :title="title"
			 :views="views"
			 :name="name"
			/>
		</div>
		
	</section> 	
	</div>
</template>

<script>
import Header from '../components/Header.vue';
import SingleCard from '../components/SingleCard.vue';
export default {
  components: {
		Header,
	SingleCard
	},
	data() {
		const singleCardData = [
			{title:"Arslan",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
			{title:"outfilters",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/mountains.jpg"
			},
			{title:"outfilters",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
			{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
			{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
			{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/quasar.jpg"
			},
			{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
			{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/parallax1.jpg"
			},
		// 	{title:"single",name:"usman",profileImage:"https://t4.ftcdn.net/jpg/03/64/21/11/360_F_364211147_1qgLVxv1Tcq0Ohz3FawUfrtONzz8nq3e.jpg",views:100,image:"https://cdn.quasar.dev/img/quasar.jpg"
		// },
		]
		return {
		singleCardData
	 }
  }
}
</script>
