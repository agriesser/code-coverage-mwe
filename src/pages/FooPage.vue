<template>
    <div>
        <h1>Foo Page</h1>
        <p>
            Counter's value is
            <span class="counter">{{ counter }}</span
            >.
        </p>
        <button @click="incrementCounter">Increment counter</button>
    </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

@Component({})
export default class FooPage extends Vue {
    counter = 0;

    incrementCounter(): void {
        this.counter += 1;
    }
}
</script>
