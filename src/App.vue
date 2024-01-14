<script setup>
    import AppBanner from '@/components/AppBanner.vue';
    import AppNavigationBar from '@/components/AppNavigationBar.vue';
    import AppCard from '@/components/AppCard.vue';
    import InformationDetail from '@/components/InformationDetail.vue';
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
                <div class="flex flex-row flex-nowrap gap-x-[64px] mb-[56px]">
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
                    <div class="w-[488px]">
                       <div class="flex flex-row">
                            <div class="flex flex-col gap-y-8 w-1/2">
                                <div>
                                    <InformationDetail label="TELEFOON" content="030-3690059"/>
                                </div>
                                <div>
                                    <InformationDetail label="INSTAGRAM">
                                        <a href="#" class="mb-0 underline text-[#006FEB]">@voelbaltrips</a>
                                    </InformationDetail>
                                </div>
                                <div>
                                    <InformationDetail label="KVK-NUMMER" content="030-3690059"/>
                                </div>
                                <div>
                                    <InformationDetail label="ONS ADRES">
                                        <p class="mb-0">
                                            Bisonspoor 332, <br>
                                            3605JT, Maarssen
                                        </p>
                                    </InformationDetail>
                                </div>
                            </div>
                            <div class="flex flex-col gap-y-8 w-1/2">
                                <div>
                                    <InformationDetail label="E-Mail" content="info@voelbaltrips.com"/>
                                </div>
                                <div>
                                    <InformationDetail label="INSTAGRAM">
                                        <a href="#" class="mb-0 underline text-[#006FEB]">Voelbaltrips.com</a>
                                    </InformationDetail>
                                </div>
                                <div>
                                    <InformationDetail label="BTW-NUMMER" content="NL859888216B01"/>
                                </div>
                            </div>
                       </div>
                    </div>
                </div>
                <img src="@/assets/map-large.png" class="w-full" alt="">
            </div>
        </div>
        <!-- End main content -->
    </div>
</template>