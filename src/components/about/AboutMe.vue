<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio: 'Hola , Influencersweb3 te conecta con la nueva tecnología emergente del momento , te llevamos de las mejores estrategias que existen en este momento. Te asesoramos sobre lo que tu negocio necesita en todos los campos del comercio, marketing digital, tecnología, inteligencia artificial (IA). Crece y  aprende temas nuevos en nuestro newsletter.  Bienvenido a este nuevo emprendimiento. '
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/teamEquip.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-6 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
