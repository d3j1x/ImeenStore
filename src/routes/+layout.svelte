<script>
    import "../app.css";
    import islogo from "$lib/img/sss.png";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';

</script>

<img src={islogo} class="flex justify-center items-center mx-auto max-h-28 rounded-full" alt="Imeen Store Logo" />

<Navbar style="font-family: 'Reem Kufi Fun', sans-serif;" >
    <NavBrand href="/">
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">متجر إيـمان</span>
    </NavBrand>
    <NavHamburger  />
    <NavUl >
      <NavLi href="/">الرئيسية</NavLi>
      <NavLi href="/">لباس شرعي</NavLi>
      <NavLi href="/">مكملات</NavLi>
      <NavLi href="/">اتصال</NavLi>
    </NavUl>
  </Navbar>


<slot></slot>

