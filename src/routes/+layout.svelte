<script>
    import "../app.css";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';

    let x =true;
    const ToOther = () => {
      setTimeout(() => {
        x = false; 
      }, 2222); 
    };

  ToOther();


</script>



{#if x}
    <div class="h-screen  text-center justify-center items-center self-center content-center mx-20">
      <h1 style="font-family: 'Reem Kufi Fun', sans-serif;" 
          class="animate-bounce rounded text-7xl shadow-2xl border-2 border-black p-10">
          <span class="">متجر إيـمـان</span>
        </h1>

    </div>


{:else}

<Navbar style="font-family: 'Reem Kufi Fun', sans-serif;" class="my-2" >
    <NavBrand href="/">
      <span class="self-center whitespace-nowrap text-2xl md:text-3xl font-semibold dark:text-white">متجر إيـمـان</span>
    </NavBrand>
    <NavHamburger  />
    <NavUl class="text-xl" >
      <NavLi class="md:text-xl" href="/">الرئيسية</NavLi>
      <NavLi class="md:text-xl" href="/">لباس شرعي</NavLi>
      <NavLi class="md:text-xl" href="/">مكملات</NavLi>
      <NavLi class="md:text-xl" href="/contact">اتصال</NavLi>
    </NavUl>
</Navbar>

<slot></slot>
  
{/if}











