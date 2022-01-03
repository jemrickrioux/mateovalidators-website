<template>
    <div class="parent">
        <div class="validator-container">
            <div>{{ node.name }}</div>
            <div :class="node.status">{{ node.status }}</div>
        </div>
        <a class="link" v-if="node.link != ''"  :href="node.link" target="__blank__"> View on Ping.pub </a>
    </div>
</template>

<script>
export default {
    name: 'Validator', 
    props: { 
        node: {
            type: Object,
            default: () => {
                return {
                    name: '',
                    status: '',
                    link: '',
                    address: '',
                }
            }
        }
    }
}
</script>

<style scoped>
.active { color: #2edf69; display: flex; justify-self: end; } 
.unbounded { color: #bc2edf; display: flex; justify-self: end; } 
.inactive { color: #d11a32; display: flex; justify-self: end; } a { color: inherit; text-decoration: none; }
h3 { font-size: 2em; } 
.validator-container {
    flex-grow: 1;
    font-size: 1.5em; 
    display: flex; 
    justify-content: space-between; 
    flex-direction: row; 
    color: white; 
}
.parent {
    padding-top: 0.5em;
}

a { color: white; text-decoration: none; }


a:hover { color: rgb(61, 212, 137); text-decoration: underline; }

.link {
    font-size: 0.75em;
}

</style>