<template>
	<a href="#" @click="onClick">Click me!</a>
</template>

<script>
import html2pdf from 'html2pdf.js';

export default {
	name: 'HtmlToPdfBtn',
	methods: {
		onClick: function() {
			const bodyEl = document.getElementsByTagName('body')[0];
			console.debug(html2pdf);
			html2pdf(bodyEl);
		}
	}
}
</script>