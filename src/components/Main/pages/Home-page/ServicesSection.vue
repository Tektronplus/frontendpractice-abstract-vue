<template>
	<div class="container-items">
		<ServiceItem
			v-for="item in dataServiceItem"
			:key="item.id"
			:title="item.title"
			:description="item.description"
			:urlImg="item.urlImg"
			:altImg="item.altImg" />
	</div>
</template>

<script>
import ServiceItem from "./ServiceItem.vue";

export default {
	components: {
		ServiceItem,
	},
	data() {
		return {
			dataServiceItem: [
				{
					id: 1,
					title: "Using Abstract",
					description:
						"Abstract lets you manage, version, and document your designs in one place.",
					urlImg: "images/icon-using-abstract.png",
					altImg: "Using Abstract",
				},
				{
					id: 2,
					title: "Manage your account",
					description:
						"Configure your account settings, such as your email, profile details, and password.",
					urlImg: "images/icon-manage-your-account.png",
					altImg: "Manage your account",
				},
				{
					id: 3,
					title: "Manage organizations, teams, and projects",
					description:
						"Use Abstract organizations, teams, and projects to organize your people and your work.",
					urlImg: "images/icon-manage-organization.png",
					altImg: "Manage your organizations",
				},
				{
					id: 4,
					title: "Manage billing",
					description: "Change subscriptions and payment details.",
					urlImg: "images/icon-manage-billing.png",
					altImg: "Manage billing",
				},
				{
					id: 5,
					title: "Authenticate to Abstract",
					description:
						"Set up and configure SSO, SCIM, and Just-in-Time provisioning.",
					urlImg: "images/icon-authenticate-to-abstract.png",
					altImg: "Authenticate to Abstract",
				},
				{
					id: 6,
					title: "Abstract support",
					description: "Get in touch with human.",
					urlImg: "images/icon-abstract-support.png",
					altImg: "Abstract support",
				},
			],
		};
	},
};
</script>

<style scoped>
.container-items {
	display: grid;
	grid-template-columns: 1fr 1fr;
	grid-template-rows: 1fr 1fr 1fr;
	gap: 90px 30px;

	padding: 10% 12%;
}

@media (max-width: 750px) {
	.container-items {
		display: flex;
		flex-direction: column;
	}
}
</style>
