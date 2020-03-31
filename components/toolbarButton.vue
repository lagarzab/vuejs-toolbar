<template>
    <a :href='href' class='toolbar-button'>
        <div class='button'>
            <slot></slot>
        </div>
    </a>
</template>

<script>
export default {
    name: 'toolbarButton',
    data () {
        return {
            href: '#',
        }
    }
}
</script>

<style lang='scss' scoped>

    a.toolbar-button  {
        height: 100%;
        text-decoration: none;
        color: black;
    }
    a.toolbar-button:hover {
        background-color:rgba(black, .25);
    }

    div.button {
        height:100%;
        position: relative;
        display:flex;
        flex-grow: 1;
        align-items: center;
        align-content: center;
        justify-content: center;
        font-weight: bold;
        margin: 0px 15px;
    }
</style>
