<template>
    <div class="py-3 px-2 flex flex-col space-y-5">
        <AddsAddHorizontal/>
        <h1 class="text-4xl">I am Topic Details</h1>
        <div class="flex justify-between">
            <UButton color="violet">Previous</UButton>
            <UButton color="violet">Next</UButton>
        </div>
        <p class="description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus minus asperiores consequuntur maiores inventore explicabo esse tempora eaque, corrupti soluta quo obcaecati ipsa quod, exercitationem ullam laboriosam ut laborum. Ad.
        </p>

        <div>
            <EachTopicDetails/>
        </div>


    </div>
</template>
<script setup>

</script>