 <template>
    <header id="site-header" class="site-header-with-search top-0 z-50 w-full transition-all sticky
    lg:fixed lg:h-22 shadow-md bg-slate-50 p-3">
        <div class="fixed inset-0 -z-10 h-[100vh] w-full bg-black/50 hidden">

        </div>
        <div>
            <div
                class="flex w-full transform-gpu items-center justify-between bg-light px-5 transition-transform duration-300 lg:h-22 lg:px-6 2xl:px-8">
                <button
                    class="group hidden h-full w-6 shrink-0 items-center justify-center focus:text-accent focus:outline-0 ltr:mr-6 rtl:ml-6 lg:flex xl:hidden"><span
                        class="sr-only">Burger Menu</span>
                    <div class="flex w-full flex-col space-y-1.5"><span
                            class="h-0.5 w-1/2 rounded bg-gray-600 transition-all group-hover:w-full"></span><span
                            class="h-0.5 w-full rounded bg-gray-600 transition-all group-hover:w-3/4"></span><span
                            class="h-0.5 w-3/4 rounded bg-gray-600 transition-all group-hover:w-full"></span></div>
                </button>
                
                <div
                    class="flex shrink-0 grow-0 basis-auto flex-wrap items-center ltr:mr-auto rtl:ml-auto lg:w-auto lg:flex-nowrap">
                    <p class="text-emerald-700 mr-2 font-semibold">Babarich</p>
                
                    <div class="hidden ltr:ml-10 ltr:mr-auto rtl:mr-10 rtl:ml-auto xl:block">
                        <div class="relative inline-block ltr:text-left rtl:text-right" data-headlessui-state=""><button
                                class="flex h-11 shrink-0 items-center text-sm font-semibold text-heading focus:outline-0 md:text-[15px] xl:px-4 rounded border-border-200 bg-light xl:min-w-150 xl:border xl:text-accent"
                                id="headlessui-menu-button-:Rpckm:" type="button" aria-haspopup="menu"
                                aria-expanded="false" data-headlessui-state=""><span
                                    class="flex h-5 w-5 items-center justify-center ltr:mr-2 rtl:ml-2"><svg width="24"
                                        height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"
                                        class="max-h-full max-w-full">
                                        <g clip-path="url(#clip0_1004_925)">
                                            <path
                                                d="M3.19965 21.3144C2.56981 21.3133 1.96187 21.0832 1.4892 20.6669C1.01653 20.2506 0.711397 19.6766 0.630699 19.052L0.0877974 14.8126C-0.0527209 13.743 -0.0253611 12.658 0.168888 11.5969C0.515551 9.72898 1.31632 7.91174 2.48362 6.34182C2.57992 6.21209 2.72381 6.12591 2.88364 6.10227C3.04347 6.07862 3.20615 6.11943 3.33589 6.21573C3.46562 6.31202 3.55179 6.45591 3.57544 6.61574C3.59909 6.77557 3.55828 6.93825 3.46198 7.06799C2.40456 8.48951 1.68001 10.1324 1.3666 11.8191C1.19591 12.7558 1.17224 13.7133 1.29645 14.6573L1.83936 18.8967C1.88657 19.258 2.07489 19.5858 2.36314 19.8087C2.65139 20.0315 3.01613 20.1312 3.37765 20.0859L3.85122 20.0255C3.93044 20.0154 4.01089 20.0209 4.08796 20.0419C4.16503 20.0629 4.23721 20.0988 4.30039 20.1477C4.36356 20.1966 4.4165 20.2574 4.45616 20.3267C4.49583 20.3961 4.52145 20.4725 4.53157 20.5517C4.54168 20.631 4.5361 20.7114 4.51512 20.7885C4.49415 20.8656 4.4582 20.9377 4.40933 21.0009C4.36046 21.0641 4.29963 21.117 4.2303 21.1567C4.16098 21.1964 4.08452 21.222 4.00529 21.2321L3.53172 21.2925C3.42161 21.3069 3.31069 21.3142 3.19965 21.3144Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M6.52299 23.999C6.30314 23.9989 6.08509 23.9595 5.87913 23.8826C5.22391 23.6369 4.74994 23.3746 4.46977 23.103C3.87138 22.52 3.48772 21.7518 3.38113 20.9232L2.79728 16.3497C2.69257 15.5209 2.87118 14.681 3.30409 13.9665C3.50682 13.6332 3.90011 13.2598 4.47301 12.8571C4.73073 12.6756 5.03101 12.5637 5.3447 12.5325C5.65839 12.5012 5.97484 12.5515 6.26334 12.6786C6.55183 12.8057 6.80257 13.0052 6.99121 13.2578C7.17986 13.5104 7.3 13.8074 7.33998 14.1201L8.33901 21.9389C8.37197 22.1966 8.34963 22.4583 8.27348 22.7067C8.19733 22.9551 8.06913 23.1844 7.89741 23.3793C7.72569 23.5742 7.51439 23.7303 7.27761 23.8372C7.04082 23.944 6.78398 23.9992 6.5242 23.999H6.52299ZM5.31757 22.2304C5.37393 22.2852 5.61112 22.483 6.30607 22.7433C6.40483 22.7809 6.51162 22.7922 6.61608 22.7763C6.72053 22.7604 6.81908 22.7177 6.90214 22.6524C6.9852 22.5871 7.04995 22.5014 7.09008 22.4036C7.13021 22.3059 7.14437 22.1994 7.13117 22.0946L6.13253 14.2742C6.1191 14.1694 6.07877 14.0698 6.01545 13.9852C5.95212 13.9006 5.86798 13.8338 5.77119 13.7913C5.67441 13.7489 5.56828 13.7322 5.46314 13.7429C5.358 13.7537 5.25743 13.7914 5.1712 13.8525C4.56302 14.2799 4.383 14.5313 4.34246 14.5982C4.05221 15.0771 3.93247 15.6401 4.00269 16.1957L4.58654 20.7692C4.65829 21.3241 4.91548 21.8385 5.31636 22.2288L5.31757 22.2304Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M20.8005 21.3146C20.6902 21.3146 20.5799 21.3075 20.4705 21.2935L19.9965 21.2331C19.9173 21.223 19.8408 21.1973 19.7715 21.1577C19.7022 21.118 19.6413 21.0651 19.5925 21.0019C19.5436 20.9387 19.5076 20.8665 19.4867 20.7895C19.4657 20.7124 19.4601 20.632 19.4702 20.5527C19.4803 20.4735 19.506 20.397 19.5456 20.3277C19.5853 20.2584 19.6382 20.1976 19.7014 20.1487C19.7646 20.0998 19.8368 20.0639 19.9138 20.0429C19.9909 20.0219 20.0714 20.0163 20.1506 20.0264L20.6246 20.0869C20.9861 20.1322 21.3508 20.0325 21.6391 19.8097C21.9273 19.5868 22.1156 19.2589 22.1628 18.8977L22.7057 14.6582C22.83 13.7143 22.8062 12.7567 22.6352 11.8201C22.3222 10.1334 21.5976 8.49049 20.5402 7.06897C20.4439 6.93955 20.403 6.77718 20.4264 6.61758C20.4498 6.45798 20.5357 6.31422 20.6651 6.21792C20.7945 6.12162 20.9569 6.08068 21.1165 6.1041C21.2761 6.12752 21.4199 6.21338 21.5161 6.3428C22.6839 7.91272 23.4842 9.72996 23.8313 11.5979C24.0253 12.659 24.0527 13.744 23.9124 14.8135L23.3699 19.0521C23.2892 19.6769 22.984 20.2509 22.5112 20.6672C22.0385 21.0835 21.4304 21.3136 20.8005 21.3146Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M19.806 7.96067H19.7739C19.5982 7.95584 19.4253 7.91557 19.2656 7.84228C19.1058 7.76898 18.9625 7.66417 18.8442 7.53413C17.9793 6.57731 16.9233 5.81248 15.7444 5.28902C14.5656 4.76556 13.29 4.4951 12.0002 4.4951C10.7103 4.4951 9.43482 4.76556 8.25596 5.28902C7.07711 5.81248 6.02111 6.57731 5.15613 7.53413C5.03784 7.6642 4.89446 7.769 4.73462 7.84223C4.57478 7.91546 4.40178 7.95561 4.22602 7.96027C4.0516 7.96509 3.87803 7.93412 3.71604 7.86926C3.55405 7.80441 3.40706 7.70705 3.28415 7.58319C3.28318 7.58201 3.28209 7.58093 3.28091 7.57995L3.25658 7.55481L2.09334 6.39238C1.92204 6.2215 1.81666 5.99558 1.79581 5.75453C1.77496 5.51347 1.83999 5.27281 1.97941 5.07506C2.8195 3.88505 6.0238 0 12.0002 0C17.9766 0 21.1805 3.88505 22.0206 5.07425C22.1601 5.27191 22.2252 5.51251 22.2045 5.75356C22.1838 5.99461 22.0786 6.22059 21.9074 6.39157L20.7195 7.57995L20.7158 7.58319C20.5967 7.70326 20.455 7.79847 20.2988 7.86327C20.1426 7.92807 19.9751 7.96118 19.806 7.96067ZM12.0002 3.2789C13.4592 3.28128 14.9017 3.58833 16.2353 4.1804C17.5688 4.77246 18.764 5.63649 19.7443 6.71715C19.7517 6.72542 19.7607 6.7321 19.7707 6.73677C19.7808 6.74145 19.7917 6.74401 19.8027 6.74431C19.8123 6.74494 19.8218 6.74345 19.8307 6.73994C19.8396 6.73644 19.8477 6.73101 19.8542 6.72404L19.8781 6.69971L19.8818 6.69647L20.9327 5.64594C20.0541 4.45269 17.1908 1.21636 12.0002 1.21636C6.80957 1.21636 3.94869 4.45026 3.06683 5.64594L4.11817 6.69647L4.12142 6.69971L4.14534 6.72404C4.15202 6.73095 4.16012 6.73634 4.16908 6.73983C4.17803 6.74333 4.18764 6.74486 4.19724 6.74431C4.20834 6.74396 4.21925 6.74133 4.22929 6.73659C4.23933 6.73185 4.2483 6.72509 4.25562 6.71674C5.23608 5.63616 6.43137 4.77222 7.76497 4.18023C9.09858 3.58824 10.5411 3.28125 12.0002 3.2789Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M17.4771 23.999C17.2173 23.9993 16.9604 23.9441 16.7236 23.8373C16.4868 23.7305 16.2755 23.5744 16.1037 23.3794C15.932 23.1845 15.8038 22.9552 15.7277 22.7068C15.6516 22.4584 15.6293 22.1966 15.6623 21.9389L16.6609 14.1201C16.7009 13.8074 16.821 13.5104 17.0097 13.2578C17.1983 13.0052 17.4491 12.8057 17.7376 12.6786C18.0261 12.5515 18.3425 12.5012 18.6562 12.5325C18.9699 12.5637 19.2702 12.6756 19.5279 12.8571C20.1012 13.2598 20.4945 13.6332 20.6968 13.9665C21.1299 14.6809 21.3085 15.5209 21.2036 16.3497L20.6198 20.9232C20.5133 21.7519 20.1297 22.5202 19.5315 23.1034C19.2518 23.375 18.7774 23.6373 18.1222 23.883C17.9158 23.96 17.6973 23.9993 17.4771 23.999ZM18.4737 13.741C18.3246 13.7405 18.1805 13.7944 18.0684 13.8928C17.9564 13.9912 17.8842 14.1271 17.8655 14.275L16.8689 22.093C16.8557 22.1978 16.8699 22.3042 16.91 22.4019C16.9501 22.4995 17.0148 22.5852 17.0979 22.6505C17.1809 22.7158 17.2793 22.7585 17.3837 22.7745C17.4881 22.7905 17.5949 22.7792 17.6936 22.7417C18.3882 22.4818 18.6262 22.2839 18.6825 22.2288C19.0834 21.8385 19.3406 21.3241 19.4123 20.7692L19.9966 16.1957C20.0666 15.6401 19.9468 15.0772 19.6568 14.5982C19.6163 14.5313 19.4362 14.2799 18.8281 13.8525C18.7242 13.7797 18.6005 13.7405 18.4737 13.7402V13.741Z"
                                                fill="currentColor"></path>
                                        </g>
                                    </svg></span><span class="whitespace-nowrap">Gadget</span><span
                                    class="flex pt-1 ltr:ml-auto ltr:pl-2.5 rtl:mr-auto rtl:pr-2.5"><svg width="10"
                                        height="6" viewBox="0 0 10 6">
                                        <path d="M128,192l5,5,5-5Z" transform="translate(-128 -192)"
                                            fill="currentColor"></path>
                                    </svg></span></button></div>
                    </div>
                </div>
                <div class="flex shrink-0 items-center space-x-7 rtl:space-x-reverse 2xl:space-x-10">
                    <ul class="hidden shrink-0 items-center space-x-7 rtl:space-x-reverse xl:flex 2xl:space-x-10">
                        <li><a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                href="#">Shops</a></li>
                        <li><a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                href="#">Offers</a></li>
                        <li><a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                href="#">Contact</a></li>
                        <li class="menuItem group relative mx-3 cursor-pointer py-3 xl:mx-4">
                            <div class="flex items-center gap-2 group-hover:text-accent"><span
                                    class="text-brand-dark group-hover:text-brand relative inline-flex items-center py-2 font-normal rtl:left-0">Pages</span><svg
                                    xmlns="http://www.w3.org/2000/svg" viewBox="0 0 12 7.2" width="12" height="7.2"
                                    class="mt-1">
                                    <path
                                        d="M6.002 5.03L10.539.265a.826.826 0 011.211 0 .94.94 0 010 1.275l-5.141 5.4a.827.827 0 01-1.183.026L.249 1.545a.937.937 0 010-1.275.826.826 0 011.211 0z"
                                        fill="currentColor"></path>
                                </svg></div>
                            <ul
                                class="shadow-dropDown invisible absolute top-full z-30 w-[220px] rounded-md bg-white py-4 opacity-0 shadow transition-all duration-300 group-hover:visible group-hover:opacity-100 ltr:left-0 rtl:right-0 xl:w-[240px]">
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/flash-sales">Flash Sale</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/manufacturers">Manufacturers/Publishers</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/authors">Authors</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/help">FAQ</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/terms">Terms &amp; Conditions</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/customer-refund-policies">Customer Refund Policy</a></li>
                                <li
                                    class="menu-child-item font-chivo hover:filter-green group py-[10px] px-[22px] transition-all duration-200 hover:pl-[25px] hover:opacity-100">
                                    <a class="flex items-center font-normal text-heading no-underline transition duration-200 hover:text-accent focus:text-accent"
                                        href="/vendor-refund-policies">Vendor Refund Policy</a></li>
                            </ul>
                        </li>
                    </ul>
                    <div class="flex items-center space-x-4 rtl:space-x-reverse"><button data-variant="custom"
                            class="inline-flex items-center justify-center shrink-0 font-semibold leading-none rounded outline-none transition duration-300 ease-in-out focus:outline-0 focus:shadow focus:ring-1 focus:ring-accent-700 px-5 py-0 h-12 hidden h-[38px] w-[38px] items-center  gap-2 rounded-full border border-border-200 bg-light !p-1 text-sm !font-normal focus:!shadow-none focus:!ring-0 md:text-base lg:!flex"><svg
                                viewBox="0 0 17.048 18" class="h-4 w-4">
                                <path
                                    d="M380.321,383.992l3.225,3.218c.167.167.341.329.5.506a.894.894,0,1,1-1.286,1.238c-1.087-1.067-2.179-2.131-3.227-3.236a.924.924,0,0,0-1.325-.222,7.509,7.509,0,1,1-3.3-14.207,7.532,7.532,0,0,1,6,11.936C380.736,383.462,380.552,383.685,380.321,383.992Zm-5.537.521a5.707,5.707,0,1,0-5.675-5.72A5.675,5.675,0,0,0,374.784,384.513Z"
                                    transform="translate(-367.297 -371.285)" fill="currentColor"></path>
                            </svg></button>
                        <div class="relative flex justify-center lg:w-auto lg:border-none flex"><button
                                data-variant="custom"
                                class="inline-flex items-center justify-center shrink-0 font-semibold leading-none rounded outline-none transition duration-300 ease-in-out focus:outline-0 focus:shadow focus:ring-1 focus:ring-accent-700 px-5 py-0 h-12 !flex h-[38px] w-[38px] max-w-full items-center gap-2 rounded-full border border-border-200 bg-light !p-1 text-sm !font-normal focus:!shadow-none focus:!ring-0 md:text-base"><span
                                    class="flex shrink-0 grow-0 basis-auto items-center gap-1 text-base text-gray-700"><svg
                                        viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"
                                        class="h-5 w-5 ">
                                        <path
                                            d="M12 0C7.34756 0 3.5625 3.78506 3.5625 8.4375C3.5625 10.0094 3.99792 11.5434 4.82198 12.8743L11.5197 23.6676C11.648 23.8744 11.874 24 12.1171 24C12.119 24 12.1208 24 12.1227 24C12.3679 23.9981 12.5944 23.8686 12.7204 23.6582L19.2474 12.7603C20.026 11.4576 20.4375 9.96277 20.4375 8.4375C20.4375 3.78506 16.6524 0 12 0ZM18.0406 12.0383L12.1065 21.9462L6.0172 12.1334C5.33128 11.0257 4.95938 9.74766 4.95938 8.4375C4.95938 4.56047 8.12297 1.39687 12 1.39687C15.877 1.39687 19.0359 4.56047 19.0359 8.4375C19.0359 9.7088 18.6885 10.9541 18.0406 12.0383Z"
                                            fill="currentColor"></path>
                                        <path
                                            d="M12 4.21875C9.67378 4.21875 7.78125 6.11128 7.78125 8.4375C7.78125 10.7489 9.64298 12.6562 12 12.6562C14.3861 12.6562 16.2188 10.7235 16.2188 8.4375C16.2188 6.11128 14.3262 4.21875 12 4.21875ZM12 11.2594C10.4411 11.2594 9.17813 9.9922 9.17813 8.4375C9.17813 6.88669 10.4492 5.61563 12 5.61563C13.5508 5.61563 14.8172 6.88669 14.8172 8.4375C14.8172 9.96952 13.5836 11.2594 12 11.2594Z"
                                            fill="currentColor"></path>
                                    </svg></span></button>
                            <div
                                class="w-full border border-border-200 bg-light p-5 shadow-[-8px_8px_16px_rgba(0,0,0,0.18)] md:min-h-0 md:w-[650px] md:rounded-xl xl:w-[1076px] fixed inset-x-0 top-[60px] mx-auto bg-white lg:top-[82px] hidden">
                                <form novalidate="" class="flex h-full gap-2.5">
                                    <div class="w-full">
                                        <div class="relative">
                                            <div class=""><input type="text" name="location"
                                                    placeholder="Search location form here"
                                                    class="line-clamp-1 flex h-12 w-full appearance-none items-center rounded border border-border-base p-4 pr-9 text-sm font-medium text-heading transition duration-300 ease-in-out invalid:border-red-500 focus:border-accent focus:outline-0 focus:ring-0 pac-target-input"
                                                    value="" autocomplete="off"></div>
                                            <div
                                                class="absolute top-0 right-0 flex h-12 w-12 items-center justify-center text-accent">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16"
                                                    viewBox="0 0 24 24" stroke-width="2" stroke="currentColor"
                                                    fill="none" stroke-linecap="round" stroke-linejoin="round"
                                                    class="h-5 w-5 cursor-pointer hover:text-accent">
                                                    <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
                                                    <path d="M12 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0"></path>
                                                    <path d="M12 12m-8 0a8 8 0 1 0 16 0a8 8 0 1 0 -16 0"></path>
                                                    <path d="M12 2l0 2"></path>
                                                    <path d="M12 20l0 2"></path>
                                                    <path d="M20 12l2 0"></path>
                                                    <path d="M2 12l2 0"></path>
                                                </svg></div>
                                        </div>
                                    </div><button
                                        class="inline-flex items-center justify-center shrink-0 font-semibold leading-none rounded outline-none transition duration-300 ease-in-out focus:outline-0 focus:shadow focus:ring-1 focus:ring-accent-700 border border-border-base bg-gray-300 hover:bg-gray-300 border-border-400 text-body cursor-not-allowed px-5 py-0 h-12 h-12 w-12 !px-0"
                                        disabled=""><svg xmlns="http://www.w3.org/2000/svg" fill="none"
                                            viewBox="0 0 24 24" stroke-width="1.8" stroke="currentColor"
                                            class="h-5 w-5">
                                            <path stroke-linecap="round" stroke-linejoin="round"
                                                d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3"></path>
                                        </svg></button>
                                </form>
                            </div>
                        </div>
                        <div class="hidden lg:inline-flex"><button
                                class="inline-flex items-center justify-center shrink-0 font-semibold leading-none rounded 
                                outline-none transition duration-300 ease-in-out focus:outline-0 focus:shadow focus:ring-1 
                                focus:ring-accent-700 bg-accent text-light border border-transparent hover:bg-accent-hover px-3 p
                                y-0 h-9 text-sm h-10  bg-emerald-600 text-white">Join</button>
                        </div><a href="#" target="_blank"
                            rel="noreferrer"
                            class="hidden h-9 shrink-0 items-center justify-center rounded border border-transparent bg-emerald-600 text-white px-3 py-0 text-sm font-semibold leading-none text-light outline-none transition duration-300 ease-in-out hover:bg-accent-hover focus:shadow focus:outline-none focus:ring-1 focus:ring-accent-700 sm:inline-flex">Become
                            a Seller</a>
                    </div>
                </div>
            </div>
        </div>
    </header>
  
   

</template>
<script setup>

</script>