<template>
    <div class="flex flex-row items-start justify-between">
        <div class="relative grow space-y-5">
            <div class="absolute top-0 bottom-0 left-0 right-0 bg-clip-content">
                <div class="relative block h-full pt-10">
                    <div class="block w-0.5 h-full blur-[0.75px] bg-orange-500 ml-[1.2rem]"></div>
                </div>
            </div>

            <!-- timeline item 1 -->
            <TimelineItem>
                <InfoCard :org="'Galaxo Smith Kline GmBH, London'" :duration="'3 years 11 months 14 days'"
                    :role="'Sales Manager (June 2020 - Present)'"
                    :summary="'Lorem ipsum dolor sit amet, consectruer adispicng elit.'" />

                <Alert :title="'Employment Gap'" :message="'26 days'" />

                <InfoCard :role="'Employment Break (March 2020 - June 2020)'"
                    :summary="'Covid 19 pandemic shutdown.'" />

                <Alert :title="'Employment Gap'" :message="'4 years 5 months 11 days'" />
            </TimelineItem>

            <!-- timeline item 2 -->
            <TimelineItem>
                <InfoCard :org="'Bigpharma Inc, London'" :duration="'3 years 9 months 25 days'"
                    :role="'Sales Executive (December 2011 - September 2015)'"
                    :summary="'Lorem ipsum dolor sit amet, consectruer adispicng elit.'" />

                <Alert :title="'Employment Gap'" :message="'3 days'" />
            </TimelineItem>

            <!-- timeline item 3 -->
            <TimelineItem>
                <InfoCard :org="'Bigpharma Inc, Essex'" :duration="'4 years 9 months 1 day'"
                    :role="'Sales Associate - Midwest Essex (March 2007 - December 2011)'"
                    :summary="'Got a promotion as sales executive.'" />
            </TimelineItem>
        </div>
    </div>
</template>

<script setup>
import TimelineItem from "@/components/TimelineItem.vue";
import InfoCard from "@/components/InfoCard.vue";
import Alert from "@/components/Alert.vue";
</script>