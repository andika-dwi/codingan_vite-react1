file Appjsx
import React from 'react'

export const App = () => {
  return (
  <html>
    <head>
      <meta charSet="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>React App</title>
    </head>
    <body>
      <header class="bg-gray-800 sticky top-0 z-50"> {/* membuat header tetap di atas saat di scroll / z-50 untuk mengatur urutan */}
        
         <nav class="text-white w-11/12 md:container mx-auto py-2 flex justify-between items-center"> {/* membuat navigasi / w-11/12 agar bisa responsive */}
          <a href="" class="text-3xl font-bold" >Home</a>
          <ul class=" md:flex space-x-4  absolute top-13 w-full left-0 bg-slate-900 divide-gray-800 divide-y-2 border"> {/* membuat menu navigasi / hidden md:flex untuk responsi */}
               <li class="px-5 py-1 hover:text-gray-500"><a href="#about">About</a></li> {/*link antar page haeus dengan # dan dengan syarat harus sama dengan id pada section */}
              <li class="px-5 py-1 hover:text-gray-500"><a href="#portofolio">Portofolio</a></li>
              <li class="px-5 py-1 hover:text-gray-500"><a href="#services">Service</a></li> {/* hover membuat text menjadi gelap saat crusor diarahkan ke text */}
              <li class="px-5 py-1 hover:text-red-800 md:hover:text-red-900"><a href="#" class="md:border-2 md:border-gray-600 md:py-1 md:px-5 md:rounded-3xl md:hover:bg-red-700 text-white">Getting Started</a></li> {/* membuat agar bisa di klik dan berwarna merah */}
          </ul>
           {/* Tombol menu */}
             <button className="hamburger-menu text-2xl text-white md:hidden">
              <i className="fa-solid fa-bars"></i>
            </button>
         </nav>

      </header>

      <section class="bg-gray-800">
        <div class="container mx-auto text-center text-white h-screen flex items-center">
          <div class="mx-auto w-2/4">  
            <h3 class="text-5xl font-bold text-center">Andika Dwi Putra</h3>
            <p class="text-gray-300 py-6 px-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit non sapiente </p>
            <a href="" class="bg-red-800 text-white py-2 px-2 rounded-2xl hover:bg-red-700">See All Portofolio</a>
          </div>
        </div>
      </section>


      
   {/* section ke 2 */}
      <section id="services" class="bg-white text-gray-700 py-20"> {/* agar bisa menyatu saat di scroll */}
        <div class="container mx-auto"> {/* agar judul pada section di tengah */}
          <h3 class="text-5xl font-bold text-center mb-5">Our Services</h3>
          <p class="text-gray-400 text-center mb-5">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nulla hic accusamus quibusdam quas delectus ut suscipit aut, praesentium culpa.</p> {/* text setelah div pertama */}


         {/* <!-- Element Di Our Services
                      1.Data Analis 
                        /Class/
                        hover:shadow-2xl transition-shadow duration-300(shadow Border didalam div)
                        flex space-x-5 py-8 px-8 bg-white rounded-xl items-start shadow-lg(Layout di dalam div)
                        <a href="" class="text-red-800">Red More</a> (agar bisa di pencet)
                      2.Text/Paragraph
                        mb-5 (margin bottom)
                        py-5 (padding top and bottom)
                        px-5 (padding left and right)

                --> */}


          <div class="grid grid-cols-2 gap-8 "> {/* membuat kolom sebelum layout */}
              
            {/* colom 1 */}
            <div class="flex space-x-5 py-8 px-8 bg-white rounded-xl items-start shadow-lg hover:shadow-2xl transition-shadow duration-300"> {/* layout didalam div /copy colom dari sini */}
              <img src="https://placehold.co/100"></img> {/* gambar di dalam div */}
              <div>
                <h4 class="text-2xl font-bold mb-5"> Data Analisis</h4>
                <p class="text-gray-500 mb-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eos dolores eveniet saepe, minus facere nihil cupiditate voluptatem, officia perferendis beatae vel excepturi nisi suscipit. Consequatur dolor repudiandae corrupti iure pariatur.</p>
                <a href="" class="text-red-800">Red More</a> {/* agar bisa di pencet */}
              </div>
            </div>


            {/* colom 2 */}
            <div class="flex space-x-5 py-8 px-8 bg-white rounded-xl items-start shadow-lg hover:shadow-2xl transition-shadow duration-300"> {/* layout didalam div /copy colom dari sini */}
              <img src="https://placehold.co/100"></img> {/* gambar di dalam div */}
              <div>
                <h4 class="text-2xl font-bold mb-5"> Sosial Media asisten</h4>
                <p class="text-gray-500 mb-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eos dolores eveniet saepe, minus facere nihil cupiditate voluptatem, officia perferendis beatae vel excepturi nisi suscipit. Consequatur dolor repudiandae corrupti iure pariatur.</p>
                <a href="" class="text-red-800">Red More</a> {/* agar bisa di pencet */}
              </div>
            </div>

            {/* colom 3 */}
            <div class="flex space-x-5 py-8 px-8 bg-white rounded-xl items-start shadow-lg hover:shadow-2xl transition-shadow duration-300"> {/* layout didalam div /copy colom dari sini */}
              <img src="https://placehold.co/100"></img> {/* gambar di dalam div */}
              <div>
                <h4 class="text-2xl font-bold mb-5"> Developer</h4>
                <p class="text-gray-500 mb-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eos dolores eveniet saepe, minus facere nihil cupiditate voluptatem, officia perferendis beatae vel excepturi nisi suscipit. Consequatur dolor repudiandae corrupti iure pariatur.</p>
                <a href="" class="text-red-800">Red More</a> {/* agar bisa di pencet */}
              </div>
            </div>

            {/* colom 4 */}
            <div class="flex space-x-5 py-8 px-8 bg-white rounded-xl items-start shadow-lg hover:shadow-2xl transition-shadow duration-300"> {/* layout didalam div /copy colom dari sini */}
              <img src="https://placehold.co/100"></img> {/* gambar di dalam div */}
              <div>
                <h4 class="text-2xl font-bold mb-5"> 24/7 proteksi </h4>
                <p class="text-gray-500 mb-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eos dolores eveniet saepe, minus facere nihil cupiditate voluptatem, officia perferendis beatae vel excepturi nisi suscipit. Consequatur dolor repudiandae corrupti iure pariatur.</p>
                <a href="" class="text-red-800">Red More</a> {/* agar bisa di pencet */}
              </div>
            </div>

          </div>
        </div>
      </section>

    {/* section ke 3 */}
      <section id="portofolio" class="py-20 bg-white">
        <h3 class="text-5xl font-bold text-center mb-5">Portofolio</h3>
        <p class="text-gray-700 mb-5 text-center">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo.</p>

        <div class="grid grid-cols-4 container mx-auto gap-6"> {/* membuat grid 4 kolom */}
          {/* portofolio 1 */}
          <div class="shadow-xl hover:shadow-2xl transition-shadow duration-500"> {/*container dengan efek shadow */}
            <a href="">
              <img src="https://placehold.co/600x400"/>
              <div class="py-3 px-5">
                <h4 class="text-center font-bold ">website pertama</h4></div>
            </a>
          </div>

          {/* portofolio 2 */}
           <div class="shadow-xl hover:shadow-2xl transition-shadow duration-500"> {/*container dengan efek shadow */}
            <a href="">
              <img src="https://placehold.co/600x400"/>
              <div class="py-3 px-5">
                <h4 class="text-center font-bold ">website kedua</h4></div>
            </a>
          </div>

          {/* portofolio 3 */}
           <div class="shadow-xl hover:shadow-2xl transition-shadow duration-500"> {/*container dengan efek shadow */}
            <a href="">
              <img src="https://placehold.co/600x400"/>
              <div class="py-3 px-5">
                <h4 class="text-center font-bold ">website ketiga</h4></div>
            </a>
          </div>

          {/* portofolio 4 */}
           <div class="shadow-xl hover:shadow-2xl transition-shadow duration-500"> {/*container dengan efek shadow */}
            <a href="">
              <img src="https://placehold.co/600x400"/>
              <div class="py-3 px-5">
                <h4 class="text-center font-bold ">website keempat</h4></div>
            </a>
          </div>
        </div>
      </section>

  {/* About */}

      <section id="about" class="container mx-auto py-20"> {/* agar bisa di tengah */}
        <div class="flex space-x-10 items-start"> {/* membuat flex agar gambar dan text bisa berdampingan */}
          <img src="https://placehold.co/300"/> {/* gambar di sebelah kiri */}
          <div> {/* text di sebelah kanan */}
            <h3 class="text-5xl font-bold mb-5">About Me</h3> {/* judul */}
            <p class="text-gray-500 mb-5 border-b pb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, voluptatum. Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, voluptatum.</p> {/* paragraf / garis bawah */}

            <ul class="flex space-x-5 mb-5 "> {/* membuat list */}
              <li><a href=""><i class="fa-brands fa-tiktok"></i></a> Tiktok</li> {/* icon tiktok */}
              <li><a href=""><i class="fa-brands fa-instagram"></i></a> Instagram</li> {/* icon instagram */}
              <li><a href=""><i class="fa-brands fa-facebook"></i></a> Facebook</li>  {/* icon facebook */}
              <li><a href=""><i class="fa-brands fa-twitter"></i></a> Twitter</li>  {/* icon twitter */}
            </ul>
            <a href="" class="bg-red-800 text-white py-2 px-5 rounded-2xl hover:bg-red-700">Read More</a> {/* agar bisa di klik */}
          </div>
        </div>
      </section>  

    </body>
    
    </html>

  )
}

export default App
