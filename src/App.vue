<script setup>
    import AppBanner from '@/components/AppBanner.vue';
    import AppNavigationBar from '@/components/AppNavigationBar.vue';
    import AppCard from '@/components/AppCard.vue';
    import ButtonPrimary from '@/components/ButtonPrimary.vue';
    import InputText from "@/components/inputs/InputText.vue"
    import InputTextarea from "@/components/inputs/InputTextarea.vue"
</script>
<template>
    <div class="main-wrapper">
        <AppBanner />
        <AppNavigationBar />

        <!-- Main content -->
        <div class="px-[100px] py-[40px]">
            <div class="container mx-auto">
                <h1 class="text-[32px] mb-8 font-medium">Neem contact op</h1>
                <div class="flex">
                    <div class="flex-1">
                        <AppCard>
                            <div class="flex flex-row gap-[15px] mb-4">
                                <div class="w-1/2">
                                    <InputText label="Naam" placeholder="Naam"/>
                                </div>
                                <div class="w-1/2">
                                    <InputText label="Email" placeholder="Email"/>
                                </div>
                            </div>
                            <div class="flex flex-row gap-[15px] mb-4">
                                <div class="w-full">
                                    <InputText label="Onderwerp" placeholder="Onderwerp"/>
                                </div>
                            </div>
                            <div class="flex flex-row gap-[15px] mb-10">
                                <div class="w-full">
                                    <InputTextarea label="Bericht" placeholder="Bericht"/>
                                </div>
                            </div>
                            <ButtonPrimary>
                                Versturen
                                <img src="@/assets/icons/arrow-right.png" class="ml-2 icon-size">
                            </ButtonPrimary>
                        </AppCard>
                    </div>
                    <div class="flex-auto"></div>
                </div>
            </div>
        </div>
        <!-- End main content -->
    </div>
</template>