<template>
    <header class="d-flex align-items-center justify-content-between">
        <div class="img-wrapper">
            <img src="../assets/img/dark-logo.png" alt="Logo MaxCoach">
        </div>

        <div class="menu ">
            <ul class="d-flex align-items-center">
                <li class="mx-4" v-for="(element, index) in menuListItems" :key=index>
                    <a href="#" class="text-black">
                        {{ element.item }}
                        <i class="fas fa-chevron-down mx-2"></i>
                    </a>
                </li>
            </ul>
        </div>

        <div class="d-flex align-items-center">
            <img src="../assets/img/en.png" alt="Logo Bandiera" class="flag">
            <p class="mx-3 my-0">English <i class="fas fa-chevron-down"></i></p>
            <i class="far fa-user-circle fs-4 mx-2"></i>

            <div class="searchbar d-flex align-items-center">
                <input type="text" placeholder="Search..." class="mx-3">
                <i class="fas fa-search fs-5 mx-2"></i>
            </div>

        </div>

    </header>
</template>

<script>
export default {
    name: 'IndexHeader',

    data: function() {
        return {
            menuListItems: [
                {
                    item: 'Home',
                },
                {
                    item: 'Pages',
                },
                {
                    item: 'Courses',
                },
                {
                    item: 'Features',
                },
                {
                    item: 'Blog',
                },
                {
                    item: 'Shop',
                }
            ],
        }
    },


}
</script>

<style lang="scss" scoped>

    header {
        height: 80px;

        & .img-wrapper {
            height: 100%;
            line-height: 75px;
            margin-left: 10rem;

            & > img {
                width: 150px;
            }
        }

        & .menu {
            ul {
                list-style-type: none;
            }

            a {
                text-decoration: none;
            }
        }

        .flag {
            height: 50%;
        }

        .searchbar {
            height: 80px;
            border-left: 1px solid lightgray;

            & input {
            border: transparent;
            }
        }

    }


</style>