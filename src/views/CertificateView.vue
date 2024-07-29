<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Rest API With Golang',
          imageUrl: 'restapi',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://www.udemy.com/certificate/UC-ef07e231-ce99-46e9-aa9d-a4b12f8b59b5/'
        },
        {
          id: 2,
          name: 'Begginer Level Golang',
          imageUrl: 'golang',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://www.udemy.com/certificate/UC-296602d7-b166-4c2b-9485-526fbe086176/'
        },
        {
          id: 3,
          name: 'Mastering PostgreSQL',
          imageUrl: 'postgre',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://udemy.com/certificate/UC-f358636d-7cd0-40cb-a4af-fddb8c413862/'
        },
        {
          id: 4,
          name: 'Basic JavaScript Programming',
          imageUrl: 'js',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/L4PQ1737OXO1'
        },
        {
          id: 5,
          name: 'Basic Structured Query Language',
          imageUrl: 'sql',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/JMZV380QJPN9'
        },
        {
          id: 6,
          name: 'Basic Google Cloud',
          imageUrl: 'gcloud',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/4EXGQ8N0GZRL'
        },
        {
          id: 7,
          name: 'SOLID Programming Principles',
          imageUrl: 'solid',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/KEXL1VN90XG2'
        },
        {
          id: 8,
          name: 'Cloud Practitioner Essentials',
          imageUrl: 'cloudaws',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/53XEO9WMKZRN'
        },
        {
          id: 9,
          name: 'Learn Basic DevOps',
          imageUrl: 'devops',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/EYX4VMYK6ZDL'
        },
        {
          id: 10,
          name: 'Make a Single Page With React',
          imageUrl: 'react',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://www.udemy.com/certificate/UC-d130bbd2-3f4f-4c78-9955-6d3c917d1b41/'
        },
        {
          id: 11,
          name: 'React Native Functions and Usage',
          imageUrl: 'native',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://www.udemy.com/certificate/UC-2428600d-fc98-432d-b0eb-79b8aa9fc01a/'
        },
        {
          id: 12,
          name: 'Introduction to Modern JavaScript',
          imageUrl: 'jsmodern',
          status: '',
          tech: 'Udemy',
          github: 'null',
          demo: 'https://www.udemy.com/certificate/UC-e83e6d68-122c-4232-9dee-cb326b5f7cd0/'
        },
        {
          id: 13,
          name: 'Basic Artificial Intelligence',
          imageUrl: 'ai',
          status: '',
          tech: 'Dicoding Academy',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/07Z60MLMYZQR'
        },
        {
          id: 14,
          name: 'Planning Career As a Software Developer',
          imageUrl: 'software',
          status: '',
          tech: 'Dicoding Indonesia',
          github: 'null',
          demo: 'https://www.dicoding.com/certificates/EYX4VMYK6ZDL'
        }
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <!-- <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"></div> -->
          <h4>Certificate Obtained</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-amber-300">
            Explore Certificates and Credential Links</h4>
        </div>
      </header>
      <section>
        <div>
          <div class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 md:gap-3 px-5 py-5 lg:px-5 ">
                <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
                  <img alt="HTML" loading="lazy" decoding="async" data-nimg="1" class="drop-shadow-xl rounded rounded-xl"
                    :src="'/img2/certificate-' + item.imageUrl + '.jpg'">
                </div>
                <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
                  <div class="title-text font-medium text-secondary">{{ item.name }}
                  </div>
                  <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                  <div class="w-full mt-4 text-normal text-sm text-left text-amber-200">
                    {{ item.tech }}
                  </div>
                  <div class="w-full flex justify-end">
                    <div class="flex cursor-pointer items-end gap-2 text-primary">
                      <a v-if="item.github !== 'null'"
                        :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                          </path>
                        </svg></a>
                        <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg></a></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </article>
</div></template>

<style>
.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}
svg:hover{
  stroke: #ffdb70;
}
@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
</style>