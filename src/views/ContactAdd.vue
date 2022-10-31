<template>
    <div class="page">
        <h4>Thêm liên hệ</h4>
         <ContactForm
        />
        <p>{{ message }}</p>
    </div>
</template>

<script>
    import ContactForm from "@/components/ContactForm.vue";
    export default {
        components: {
            ContactForm,
        },
        props: {
            id: { type: String, required: true },
        },
        data() {
            return {
                contact: null,
                message: "",
            };
        },
    }
</script>