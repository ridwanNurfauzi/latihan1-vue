<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>
<template>
    <Navbar class="sticky top-0 z-[10000] bg-opacity-70 backdrop-blur-sm">
        <template #logo>
            <NavbarLogo link="https://ridwannurfauzi.github.io/" alt="logo"
                image-url="/logo.svg"
                class="hover:opacity-95 hover:rotate-12 hover:scale-125 hover:hue-rotate-90 transition">
            </NavbarLogo>
            <slot name="title">
                Navbar
            </slot>
        </template>
        <template #default="{ isShowMenu }">
            <NavbarCollapse :isShowMenu="isShowMenu" class="mx-auto">
                <NavbarLink link="#home">Home</NavbarLink>
                <NavbarLink link="#bio">Biodata</NavbarLink>
                <NavbarLink link="#project">Project</NavbarLink>
                <NavbarLink link="#contact">Contact</NavbarLink>
            </NavbarCollapse>
        </template>
    </Navbar>
</template>
