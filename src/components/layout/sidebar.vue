<template>
    <!--  BEGIN SIDEBAR  -->
    <div class="sidebar-wrapper sidebar-theme">
        <nav ref="menu" id="sidebar">
            <div class="shadow-bottom"></div>

            <perfect-scrollbar class="list-unstyled menu-categories" tag="ul" :options="{ wheelSpeed: 0.5, swipeEasing: !0, minScrollbarLength: 40, maxScrollbarLength: 300, suppressScrollX: true }">
                <li class="menu">
                    <a class="dropdown-toggle" data-bs-toggle="collapse" data-bs-target="#dashboard" aria-controls="dashboard" aria-expanded="false">
                        <div class="">
                            <svg
                                    xmlns="http://www.w3.org/2000/svg"
                                    width="24"
                                    height="24"
                                    viewBox="0 0 24 24"
                                    fill="none"
                                    stroke="currentColor"
                                    stroke-width="2"
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                    class="feather feather-plus"
                                >
                                    <line x1="12" y1="5" x2="12" y2="19"></line>
                                    <line x1="5" y1="12" x2="19" y2="12"></line>
                                </svg>
                            <span>Nuevo</span>
                        </div>
                        <div>
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                width="24"
                                height="24"
                                viewBox="0 0 24 24"
                                fill="none"
                                stroke="currentColor"
                                stroke-width="2"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                class="feather feather-chevron-right"
                            >
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </div>
                    </a>
                </li>

                <li class="menu">
                    <a class="dropdown-toggle" data-bs-toggle="collapse" data-bs-target="#apps" aria-controls="apps" aria-expanded="false">
                        <div class="">
                            <svg xmlns="http://www.w3.org/2000/svg" 
                                width="24" 
                                height="24" 
                                viewBox="0 0 24 24" 
                                fill="none" 
                                stroke="currentColor" 
                                stroke-width="2" 
                                stroke-linecap="round" 
                                stroke-linejoin="round" 
                                class="feather feather-clock">
                                <circle cx="12" cy="12" r="10"></circle>
                                <polyline points="12 6 12 12 16 14"></polyline>
                            </svg>
                            <span>Historial</span>
                        </div>
                        <div>
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                width="24"
                                height="24"
                                viewBox="0 0 24 24"
                                fill="none"
                                stroke="currentColor"
                                stroke-width="2"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                class="feather feather-chevron-right"
                            >
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </div>
                    </a>
                     <ul id="apps" class="collapse submenu list-unstyled" data-bs-parent="#sidebar">
                        <li>
                            <a class="dropdown-toggle" href="#favoritos" data-bs-parent="#apps" data-bs-toggle="collapse" role="button" aria-expanded="false">
                                Favoritos
                                <svg
                                    xmlns="http://www.w3.org/2000/svg"
                                    width="24"
                                    height="24"
                                    viewBox="0 0 24 24"
                                    fill="none"
                                    stroke="currentColor"
                                    stroke-width="2"
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                    class="feather feather-chevron-right"
                                >
                                    <polyline points="9 18 15 12 9 6"></polyline>
                                </svg>
                            </a>
                            <ul id="favoritos" class="collapse list-unstyled sub-submenu">
                                <li>
                                    <router-link to="#" @click="toggleMobileMenu">Sentencia</router-link>
                                </li>
                            </ul>
                        </li>
                        <li>
                            <a class="dropdown-toggle" href="#recientes" data-bs-parent="#apps" data-bs-toggle="collapse" role="button" aria-expanded="false">
                                Recientes
                                <svg
                                    xmlns="http://www.w3.org/2000/svg"
                                    width="24"
                                    height="24"
                                    viewBox="0 0 24 24"
                                    fill="none"
                                    stroke="currentColor"
                                    stroke-width="2"
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                    class="feather feather-chevron-right"
                                >
                                    <polyline points="9 18 15 12 9 6"></polyline>
                                </svg>
                            </a>

                            <ul id="recientes" class="collapse list-unstyled sub-submenu">
                                <li>
                                    <a class="dropdown-toggle" href="#ayer" data-bs-parent="#apps" data-bs-toggle="collapse" role="button" aria-expanded="false">
                                        Ayer
                                        <svg
                                            xmlns="http://www.w3.org/2000/svg"
                                            width="24"
                                            height="24"
                                            viewBox="0 0 24 24"
                                            fill="none"
                                            stroke="currentColor"
                                            stroke-width="2"
                                            stroke-linecap="round"
                                            stroke-linejoin="round"
                                            class="feather feather-chevron-right"
                                        >
                                            <polyline points="9 18 15 12 9 6"></polyline>
                                        </svg>
                                    </a>
                                    <ul id="ayer" class="collapse list-unstyled sub-submenu">
                                        <li>
                                            <router-link to="#" @click="toggleMobileMenu">Protección derechos políticos-electorales</router-link>
                                        </li>
                                    </ul>
                                    
                                </li>
                                <li>
                                    <a class="dropdown-toggle" href="#siete-dias" data-bs-parent="#apps" data-bs-toggle="collapse" role="button" aria-expanded="false">
                                        Últimos 7 días
                                        <svg
                                            xmlns="http://www.w3.org/2000/svg"
                                            width="24"
                                            height="24"
                                            viewBox="0 0 24 24"
                                            fill="none"
                                            stroke="currentColor"
                                            stroke-width="2"
                                            stroke-linecap="round"
                                            stroke-linejoin="round"
                                            class="feather feather-chevron-right"
                                        >
                                            <polyline points="9 18 15 12 9 6"></polyline>
                                        </svg>
                                    </a>
                                    <ul id="siete-dias" class="collapse list-unstyled sub-submenu">
                                        <li>
                                            <router-link to="#" @click="toggleMobileMenu"></router-link>
                                        </li>
                                    </ul>
                                </li>
                                <li>
                                    <a class="dropdown-toggle" href="#treinta-dias" data-bs-parent="#apps" data-bs-toggle="collapse" role="button" aria-expanded="false">
                                        Últimos 30 días
                                        <svg
                                            xmlns="http://www.w3.org/2000/svg"
                                            width="24"
                                            height="24"
                                            viewBox="0 0 24 24"
                                            fill="none"
                                            stroke="currentColor"
                                            stroke-width="2"
                                            stroke-linecap="round"
                                            stroke-linejoin="round"
                                            class="feather feather-chevron-right"
                                        >
                                            <polyline points="9 18 15 12 9 6"></polyline>
                                        </svg>
                                    </a>
                                    <ul id="treinta-dias" class="collapse list-unstyled sub-submenu">
                                        <li>
                                            <router-link to="#" @click="toggleMobileMenu"></router-link>
                                        </li>
                                    </ul>
                                </li>
                            </ul>
                        </li>
                    </ul> 
                </li> 
            </perfect-scrollbar>
        </nav>
    </div>
    <!--  END SIDEBAR  -->
</template>

<script setup>
    import { onMounted, ref } from 'vue';
    import { useStore } from 'vuex';
    //import chat from '@/views/apps/chat.vue';
    const store = useStore();

    const menu_collapse = ref('dashboard');
    //const select_user = chat.select_user;

    onMounted(() => {
        const selector = document.querySelector('#sidebar a[href="' + window.location.pathname + '"]');
        if (selector) {
            const ul = selector.closest('ul.collapse');
            if (ul) {
                let ele = ul.closest('li.menu').querySelectorAll('.dropdown-toggle');
                if (ele) {
                    ele = ele[0];
                    setTimeout(() => {
                        ele.click();
                    });
                }
            } else {
                selector.click();
            }
        }
    });

    const toggleMobileMenu = () => {
        if (window.innerWidth < 991) {
            store.commit('toggleSideBar', !store.state.is_show_sidebar);
        }
    };
</script>
