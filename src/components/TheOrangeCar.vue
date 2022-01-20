<template>
<svg viewBox="0 0 240 277" class="orange-car" :style="`left:${leftPosition}; top: ${topPosition}; height: ${heightSize} `">
	<title>The Orange Car</title>
	<defs>
		<linearGradient id="orangeCar1" x1="39" y1="140.9" x2="39" y2="162.8" gradientUnits="userSpaceOnUse">
			<stop offset=".1" stop-color="#fcee21"/>
			<stop offset=".7" stop-color="#f77f0f"/>
		</linearGradient>
		<linearGradient id="orangeCar2" x1="-1.5" y1="167.3" x2="-1.5" y2="142.4" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#00b8c4"/>
			<stop offset=".3" stop-color="#83f7c7"/>
			<stop offset="1" stop-color="#00b8c4"/>
		</linearGradient>
		<linearGradient id="orangeCar3" x1="200.8" y1="140.9" x2="200.8" y2="162.8" gradientUnits="userSpaceOnUse">
			<stop offset=".1" stop-color="#fcee21"/>
			<stop offset=".7" stop-color="#f77f0f"/>
		</linearGradient>
		<linearGradient id="orangeCar4" x1="241.3" y1="167.3" x2="241.3" y2="142.4" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#00b8c4"/>
			<stop offset=".3" stop-color="#83f7c7"/>
			<stop offset="1" stop-color="#00b8c4"/>
		</linearGradient>
		<linearGradient id="orangeCar5" x1="36.2" y1="168.8" x2="36.2" y2="3.2" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#00b8c4"/>
			<stop offset=".3" stop-color="#83f7c7"/>
			<stop offset="1" stop-color="#00b8c4"/>
		</linearGradient>
		<linearGradient id="orangeCar6" x1="38.1" y1="157" x2="38.1" y2="94" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#83f7c7"/>
			<stop offset=".7" stop-color="#00b8c4"/>
		</linearGradient>
		<linearGradient id="orangeCar7" x1="213.6" y1="-4.3" x2="209.1" y2="159.4" gradientUnits="userSpaceOnUse">
			<stop offset=".1" stop-color="#fcee21"/>
			<stop offset=".7" stop-color="#f77f0f"/>
		</linearGradient>
		<linearGradient id="orangeCar8" x1="228.4" y1="144.4" x2="228.4" y2="264.3" gradientUnits="userSpaceOnUse">
			<stop offset=".1" stop-color="#fcee21"/>
			<stop offset=".7" stop-color="#f77f0f"/>
		</linearGradient>
		<linearGradient id="orangeCar9" x1="58.8" y1="249.7" x2="58.8" y2="273" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#131f49"/>
			<stop offset=".9" stop-color="#14466a"/>
			<stop offset="1" stop-color="#22567d"/>
		</linearGradient>
		<linearGradient id="orangeCar10" x1="180.8" y1="249.7" x2="180.8" y2="273" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#131f49"/>
			<stop offset=".9" stop-color="#14466a"/>
			<stop offset="1" stop-color="#22567d"/>
		</linearGradient>
		<linearGradient id="orangeCar11" x1="12.2" y1="224.4" x2="11.3" y2="197.5" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#e7855f"/>
			<stop offset="1" stop-color="#9a1418"/>
		</linearGradient>
		<linearGradient id="orangeCar12" x1="13.6" y1="207.3" x2="16.4" y2="144.3" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#fff7cc"/>
			<stop offset="1" stop-color="#fff7cc"/>
		</linearGradient>
		<linearGradient id="orangeCar13" x1="225.4" y1="207.2" x2="221.9" y2="144.1" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#fff7cc"/>
			<stop offset="1" stop-color="#fff7cc"/>
		</linearGradient>
		<linearGradient id="orangeCar14" x1="36.3" y1="212.8" x2="36.1" y2="151.5" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#fff7cc"/>
			<stop offset="1" stop-color="#fff7cc"/>
		</linearGradient>
		<linearGradient id="orangeCar15" x1="117.5" y1="212.4" x2="117.3" y2="151.7" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#fff7cc"/>
			<stop offset="1" stop-color="#fff7cc"/>
		</linearGradient>
		<linearGradient id="orangeCar16" x1="35.5" y1="123.8" x2="35.5" y2="-5.8" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#fff7cc"/>
			<stop offset="1" stop-color="#fff7cc"/>
		</linearGradient>
		<linearGradient id="orangeCar17" x1="227.9" y1="224.4" x2="228.8" y2="197.5" gradientUnits="userSpaceOnUse">
			<stop offset="0" stop-color="#e7855f"/>
			<stop offset="1" stop-color="#9a1418"/>
		</linearGradient>
	</defs>

	<g>
		<g>
			<path  class="s0" d="m31.2 161.7c-9.5 1-18.2 1.6-25.6 1.2c-4.3-5.6-6.1-12-4.6-19.6c8.7-2.1 17.9-1.9 27.4 0c2.6 2.4 4.7 6.4 6.7 10.9z" />
			<path  class="s1" d="m10.5 161.1q-2 0-3.9-0.1c-3.6-4.8-4.8-10.1-3.9-16.1c3.6-0.8 7.5-1.2 11.4-1.2c4.2 0 8.7 0.5 13.4 1.4c2.2 2.3 4.1 6.1 5.5 9.1l-3 5.7c-7.8 0.8-14.1 1.2-19.5 1.2z" />
			<path  class="s2" d="m2.7 144.9c6.8-1.8 15.2-1.3 24.8 0.2c1.9 2.5 4.1 5.6 5.5 9.1q-2.3-2.7-7.3-6.6q-14.1-2-23-2.7z" />
			<path  fill-rule="evenodd" class="s3" d="m20.1 145.1l5 14.3l-4.2 0.3l-10.8-14.9zm4.9 0.6l2.2 13.8h-1.3l-4.8-14.1z" />
			<path  class="s4" d="m204.7 154.2c2-4.5 4.2-8.5 6.7-10.9c9.6-1.9 18.7-2.1 27.4 0c1.5 7.6-0.2 14-4.6 19.6c-7.3 0.4-16.1-0.2-25.5-1.2z" />
			<path  class="s5" d="m209.9 159.9l-3.1-5.7c1.4-3 3.3-6.8 5.6-9.1c4.6-0.9 9.1-1.4 13.3-1.4c4 0 7.8 0.4 11.4 1.2c1 6-0.3 11.3-3.9 16.1q-1.8 0.1-3.9 0.1c-5.3 0-11.7-0.4-19.4-1.2z" />
			<path  class="s2" d="m214.1 147.6q-5 3.9-7.3 6.6c1.5-3.5 3.6-6.6 5.6-9.1c9.5-1.5 17.9-2 24.7-0.2q-8.8 0.7-23 2.7z" />
			<path  fill-rule="evenodd" class="s3" d="m229.8 144.8l-10.9 14.9l-4.1-0.3l4.9-14.3zm-11.1 0.5l-4.8 14.1h-1.3l2.2-13.8z" />
			<path  class="s6" d="m199.8 149.8q-79.8 15.9-159.6 0c5-54.3 13.3-105.8 25.5-139q54.3-6.1 108.6 0c12.2 33.2 20.5 84.7 25.5 139z" />
			<path  class="s7" d="m42.1 148.1l8.9-61.4h20.9v20.9h5.7v28.1h3.1v-20.4h3.8v-20.2l14-1.1v37.6h1.9v-22.8l11.4-1.2v9.8h6.5l0.9 10l4-0.8l-1.2-30l16.4-1.9v-8h14v11.4l8 0.4v26.6l4.6-0.8v-17l10.9-0.8v-13.7l6.9-0.4l-1.3-9.6h6.7l9.3 64.8c-52.5 10.4-104.2 10.5-155.4 0.5z" />
			<path  class="s8" d="m205.4 148.6l-5.6 1.2c-5-54.3-13.3-105.8-25.5-139q-54.3-6.1-108.6 0c-12.2 33.2-20.5 84.7-25.5 139l-5.6-1.6c4.3-51.5 10.9-97.9 22.1-134.8l-1.3-7.6c18.6-4.2 40.8-5.5 64.6-5.5c23.8 0 46 1.3 64.5 5.5l-1.2 7.6c11.2 36.9 17.9 83.6 22.1 135.2z" />
			<path  class="s9" d="m221.3 224.6c4.1 9.6 2.8 18.5-5.5 26.3c-63.2 2.4-127.1 2.4-191.6 0c-8.3-7.8-9.6-16.7-5.5-26.3c-2.7-10.1-3.7-19.9-2.8-29.6c4.9-14.1 11.1-27.6 18.3-40.8q0.2-3 0.4-6l5.6 1.6h159.6l5.6-1.2q0.2 2.8 0.4 5.6c7.1 13.2 13.3 26.7 18.3 40.8c0.9 9.7-0.1 19.5-2.8 29.6z" />
			<path  class="s10" d="m54.8 251.9c-0.3 5.2-1.4 11.3-3.1 17.9c-0.1 0.5-0.6 0.9-1.1 0.9h-15.4c-0.5 0-1-0.3-1.2-0.8c-1.9-6-3.4-12.2-4.5-18.8z" />
			<path  class="s11" d="m210.1 251.1c-1 6.6-2.5 12.8-4.5 18.8c-0.2 0.5-0.6 0.8-1.1 0.8h-15.4c-0.6 0-1.1-0.4-1.2-0.9c-1.6-6.6-2.8-12.7-3.1-17.9z" />
			<path  class="s12" d="m54.8 202.4q1.1 13.7 3.3 20.2c-10.7 3.3-26.3 3.8-39.4 2c-3.1-9-3.3-18.4-2.8-29.3c13.1-0.4 39.2 5.8 38.9 7.1z" />
			<path  class="s13" d="m37.9 150.5c0 20.4 6.4 37 15.4 49.2c-9.4-4.1-21.7-6.6-35.1-6.5c4.9-13.7 10.9-28.3 17.7-43.4z" />
			<path  class="s14" d="m203.1 149.8c6.7 15.1 12.6 29.5 17.5 43.2c-12.9 0-24.6 2.7-33.6 6.8c8.5-12.2 14.5-28.8 14.3-49.2z" />
			<g >
				<path  class="s15" d="m121.3 160.6l0.1 38l-66.3-0.6c-11.3-13.9-15.8-30.1-14.9-46.4z" />
				<path  class="s16" d="m185.1 198l-63.7 0.6l0.1-38l77.8-9c0.9 16.3-3.4 32.5-14.2 46.4z" />
			</g>
			<path  class="s3" d="m60.1 221.6h119.9q-40.1 3.4-59.2 4q-19 0.5-60.7-4z" />
			<path  class="s2" d="m25.9 246.3c58.6 1.6 120.6 1.3 185.4-0.6c4.7-2.3 7.6-6.6 9.3-12c0.3 5.7-1.2 11-6.5 15.4c-67.2 2.5-130.9 2.9-189.4 0c-2.9-2.8-5.1-6.1-6-10z" />
			<path  class="s2" d="m38.9 159.4c0.5 14.4 6.6 27.2 15.9 39.2c-7.7-13.2-13.6-26.3-15.9-39.2z" />
			<path  class="s2" d="m201.2 159.4c-0.5 14.4-6.6 27.2-16 39.2c7.7-13.2 13.7-26.3 16-39.2z" />
			<path  class="s3" d="m20.2 226.1q11.6 1.8 19.9 1q8.3-0.7 18.5-3.5q-9.4 5.1-18.4 5.8q-8.9 0.8-20-3.3z" />
			<path  class="s3" d="m199.9 229.4q-9-0.7-18.4-5.8q10.2 2.8 18.5 3.5q8.2 0.8 19.8-1q-11 4.1-19.9 3.3z" />
			<path  class="s17" d="m182.8 7l-1.1 6.5l0.1 0.4c8 26.2 14.2 59.1 18.7 100.1q-1.4 0.7-2.9 1.3c-4.4-36.1-11.3-76.2-21.9-105l-0.3-0.9l-1-0.1c-18-2-36.3-3.1-54.4-3.1c-18.1 0-36.4 1.1-54.5 3.1l-0.9 0.1l-0.3 0.9c-10.6 28.8-17.5 68.9-21.9 105q-1.5-0.6-2.9-1.3c4.5-40.9 10.7-73.9 18.6-100.1l0.1-0.4l-1-6.5c16.1-3.5 35.9-5.2 62.1-5.2h1.4c26.2 0 46 1.7 62.1 5.2z" />
			<path  class="s2" d="m65.7 10.8l-7.2-2.3c41.2-5.7 82.3-5.9 123.3 0l-7.5 2.3c-35.8-3.5-72-3.4-108.6 0z" />
			<g >
				<path  class="s2" d="m152.6 218.8h-68.6l-1.5-13.5h73.9z" />
				<path  class="s18" d="m152.2 217.2h-67.8l-1.5-13.9h73.1z" />
				<path  class="s2" d="m85.6 215l-1.1-10.6h69.4l-1 5.3l-0.5-3.4l-66.5-0.5z" />
				<path  class="s19" d="m86.5 214.8l63.6-1l0.7 2.1l-65 0.2z" />
			</g>
			<path  class="s2" d="m41.3 151.7l158-0.1q-37.9 3.2-77.9 3.9q-40 0.6-80.1-3.8z" />
			<path  class="s2" d="m46.9 144.6l68.9 3.6c-26.9 0.7-51.9 0.8-72.4-0.6c0.4-14.6 2.7-35.1 5.3-57.2z" />
			<path  class="s2" d="m191.3 90.4c2.7 22.1 4.9 42.6 5.3 57.2c-20.5 1.4-45.5 1.3-72.4 0.6l69-3.6z" />
			<path  class="s2" d="m50.3 71.9c4.4-23.6 9.4-45.1 15.4-61.1c36.7-4.1 72.9-4 108.6 0c6.8 17.1 12.1 43.8 17.2 72c-7-26.3-14.1-51.6-23.3-66.6c-32.2-3-65.5-3.3-99.7-1.5c-6.3 15-12.3 35.2-18.2 57.2z" />
			<path  fill-rule="evenodd" class="s3" d="m136.5 10.8c-15.7 36.2-31.3 85.5-46.4 137.3h-11.4c7.2-53.4 14.5-103.4 22.5-137.3q18-1.8 35.3 0zm-38.6 0.4l-22.3 136.4h-3.8l11.8-134.9q6.9-1 14.3-1.5z" />
			<path  class="s20" d="m53.8 203.3v4.7l-36.3-1.1c-0.6-3.1-0.5-6.4 0-9.9c13.2 0.9 25.3 2.9 36.3 6.3z" />
			<path  class="s21" d="m17.5 208.4l35.8 1.3l1.1 5.2l-36.2-0.4z" />
			<path  class="s22" d="m54.4 217.1l1.3 5.1c-12.3 0.8-24.2 1-35.5 0.2l-2-6.3z" />
			<path  class="s2" d="m22 220.8c8.7 1.9 21 1.8 34.1 1.3c-12.1 2.3-24.2 3.9-36.6 1.7c-0.7-1.8-1.6-4.9-2-6.7c1.4 1.3 3 2.6 4.5 3.7z" />
			<path  class="s3" d="m18.2 214.5l-0.7-17.5c11.6 0.3 23.8 2.7 36.3 6.3l0.6 13.8l-4.3-11.2c-10-2-19.7-3.3-28.9-3.4z" />
			<path  class="s23" d="m224.2 195.3c0.5 10.9 0.3 20.3-2.8 29.3c-13.1 1.8-28.7 1.3-39.4-2q2.2-6.5 3.3-20.2c-0.3-1.3 25.8-7.5 38.9-7.1z" />
			<path  class="s20" d="m222.6 197c0.5 3.5 0.6 6.8 0 9.9l-36.3 1.1v-4.7c11-3.4 23.1-5.4 36.3-6.3z" />
			<path  class="s21" d="m221.9 214.5l-36.2 0.4l1.1-5.2l35.8-1.3z" />
			<path  class="s22" d="m221.9 216.1l-2 6.3c-11.3 0.8-23.2 0.6-35.5-0.2l1.3-5.1z" />
			<path  class="s2" d="m222.6 217.1c-0.4 1.8-1.3 4.9-2 6.7c-12.4 2.2-24.6 0.6-36.6-1.7c13.1 0.5 25.4 0.6 34.1-1.3c1.5-1.1 3.1-2.4 4.5-3.7z" />
			<path  class="s3" d="m218.9 202.5c-9.2 0.1-18.9 1.4-28.9 3.4l-4.3 11.2l0.6-13.8c12.5-3.6 24.7-6 36.3-6.3l-0.7 17.5z" />
			<path  class="s24" d="m119.7 264.3c56.8 0 102.9 2.8 102.9 6.4c0 3.5-46.1 6.4-102.9 6.4c-56.8 0-102.9-2.9-102.9-6.4c0-3.6 46.1-6.4 102.9-6.4z" />
		</g>
		<path  class="s25" d="m234.2 162.9c-7 0.4-15.4-0.1-24.4-1.1c5.5 10.8 10.3 21.8 14.3 33.2q0 0.1 0 0.3q0.1 0 0.1 0q0.1 3 0.2 5.8q0 0.7 0 1.5c0 7.9-0.6 15.1-3 22q0 0-0.1 0c4.1 9.6 2.8 18.5-5.5 26.3q-3.1 0.1-6.1 0.2h0.4c-1 6.6-2.5 12.8-4.5 18.8c-0.2 0.5-0.6 0.8-1.1 0.8h-15.4c-0.6 0-1.1-0.4-1.2-0.9c-1.6-6.6-2.8-12.7-3.1-17.9q-66.1 1.6-133.1-0.1l3.1 0.1c-0.3 5.2-1.4 11.3-3.1 17.9c-0.1 0.5-0.6 0.9-1.1 0.9h-15.4c-0.5 0-1-0.3-1.2-0.8c-1.9-6-3.4-12.2-4.5-18.8l8.4 0.3q-6.9-0.2-13.7-0.5c-8.3-7.8-9.6-16.7-5.5-26.3c-1.8-5.2-2.6-10.6-2.9-16.3q-0.5-6.5 0.1-12.8q0-0.1 0-0.2q0 0 0 0q0-0.2 0-0.3c4-11.4 8.8-22.4 14.3-33.2c-9.1 0.9-17.5 1.5-24.6 1.1c-4.3-5.6-6.1-12-4.6-19.6c8.7-2.1 17.9-1.9 27.4 0c2.2 2.1 4.1 5.4 5.9 9.2q0.2-2.1 0.3-4.3c4.3-51.5 10.9-97.9 22.1-134.8l-1.3-7.6c18.6-4.2 40.8-5.5 64.6-5.5c23.8 0 46 1.3 64.5 5.5l-1.2 7.6c11.2 36.9 17.9 83.6 22.1 135.2q0.1 1.8 0.2 3.6c1.8-3.7 3.7-6.8 5.8-8.9c9.6-1.9 18.7-2.1 27.4 0c1.5 7.6-0.2 14-4.6 19.6z" />
	</g>
</svg>
</template>
<script setup lang="ts">
  const props = defineProps({
  topPosition: String,
  leftPosition: String,
  heightSize: String,
})
</script>
	<style>
		.orange-car .s0 { fill: url(#orangeCar1) } 
		.orange-car .s1 { fill: url(#orangeCar2) } 
		.orange-car .s2 { opacity: .4;mix-blend-mode: multiply;fill: #b86053 } 
		.orange-car .s3 { opacity: .5;mix-blend-mode: screen;fill: #fff7cc } 
		.orange-car .s4 { fill: url(#orangeCar3) } 
		.orange-car .s5 { fill: url(#orangeCar4) } 
		.orange-car .s6 { fill: url(#orangeCar5) } 
		.orange-car .s7 { fill: url(#orangeCar6) } 
		.orange-car .s8 { fill: url(#orangeCar7) } 
		.orange-car .s9 { fill: url(#orangeCar8) } 
		.orange-car .s10 { fill: url(#orangeCar9) } 
		.orange-car .s11 { fill: url(#orangeCar10) } 
		.orange-car .s12 { fill: url(#orangeCar11) } 
		.orange-car .s13 { opacity: .7;mix-blend-mode: screen;fill: url(#orangeCar12) } 
		.orange-car .s14 { opacity: .7;mix-blend-mode: screen;fill: url(#orangeCar13) } 
		.orange-car .s15 { opacity: .7;mix-blend-mode: screen;fill: url(#orangeCar14) } 
		.orange-car .s16 { opacity: .7;mix-blend-mode: screen;fill: url(#orangeCar15) } 
		.orange-car .s17 { opacity: .7;mix-blend-mode: screen;fill: url(#orangeCar16) } 
		.orange-car .s18 { fill: #ffd699 } 
		.orange-car .s19 { fill: #fff7cc } 
		.orange-car .s20 { fill: #9a1418 } 
		.orange-car .s21 { opacity: .3;mix-blend-mode: screen;fill: #fff7cc } 
		.orange-car .s22 { fill: #d96118 } 
		.orange-car .s23 { fill: url(#orangeCar17) } 
		.orange-car .s24 { opacity: .5;mix-blend-mode: multiply;fill: #b86053 } 
		.orange-car .s25 { opacity: .6;mix-blend-mode: multiply;fill: #b86053 } 
	</style>