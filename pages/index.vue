<template>
    <section class="max-w-6xl w-full m-auto py-12">
        <h1 class="text-4xl mb-6">Welcome to Nuxt 3 Starter Pack</h1>
        <Success text="Information has been updated" />
        <Error text="Information has been updated" />
        <Processing text="File is Uploading ...." />
        <Failed text="Password & Email are wrong!" />

        <Input placeholder="Email Address" />

        <Select>
            <option value="" selected>Please select a country!</option>
            <option value="PK">Pakistan</option>
            <option value="UK">United Kingdom</option>
            <option value="US">United States</option>
            <option value="DE">Germany</option>
        </Select>

        <ClientOnly>
            <Quill id="body" v-model:content="body"/>
        </ClientOnly>

        <Textarea placeholder="Write message here..." />
    </section>
</template>

<script setup>
    const body = ref("");
</script>