<script setup>
    import AppBanner from '@/components/AppBanner.vue';
    import AppNavigationBar from '@/components/AppNavigationBar.vue';
    import AppCard from '@/components/AppCard.vue';
</script>
<template>
    <div class="main-wrapper">
        <AppBanner />
        <AppNavigationBar />

        <!-- Main content -->
        <div class="container mx-auto">
            <h1 class="text-[32px]">Neem contact op</h1>
            <div class="flex">
                <div class="flex-1">
                    <AppCard>
                        asd
                    </AppCard>
                </div>
                <div class="flex-auto"></div>
            </div>
        </div>
        
        <!-- End main content -->
    </div>
</template>