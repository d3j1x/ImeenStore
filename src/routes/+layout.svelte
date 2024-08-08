<script>
    import "../app.css";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>



<Navbar style="font-family: 'Reem Kufi Fun', sans-serif;" class="my-2" >
    <NavBrand href="/">
      <span class="self-center whitespace-nowrap text-2xl md:text-3xl font-semibold dark:text-white">متجر إيـمـان</span>
    </NavBrand>
    <NavHamburger  />
    <NavUl class="text-xl" >
      <NavLi class="md:text-xl" href="/">الرئيسية</NavLi>
      <NavLi class="md:text-xl" href="/">لباس شرعي</NavLi>
      <NavLi class="md:text-xl" href="/">مكملات</NavLi>
      <NavLi class="md:text-xl" href="/">اتصال</NavLi>
    </NavUl>
</Navbar>




<slot></slot>

