<template>
  <div class="bg-white overflow-hidden">
    <div class="relative max-w-7xl mx-auto py-0 px-4 sm:px-6 lq:px-8">
      <div class="hidden lg:block bg-gray-50 absolute top-0 bottom-0 left-3/4 w-screen" />
      <div class="mx-auto text-base max-w-prose lg:grid lg:grid-cols-2 lg:gap-8 lg:max-w-none">
        <div></div>
      </div>

      <div class="mt-8 lg:grid lg:grid-cols-1 lg:gap-2">
        <div class="text-base max-w-prose lg:max-w-none"></div>
        <div class="relative lg:row-start-1 lg:col-start-2">
          <svg
            class="hidden lg:block absolute top-0 right-0 -mt-20 -mr-20"
            width="404"
            height="384"
            fill="none"
            viewBox="0 0 404 384"
            aria-hidden="true"
          >
            <defs>
              <pattern
                id="de316486-4a29-4312-bdfc-fbce2132a2c1"
                x="0"
                y="0"
                width="20"
                height="20"
                patternUnits="userSpaceOnUse"
              >
                <rect
                  x="0"
                  y="0"
                  width="4"
                  height="4"
                  class="text-gray-200"
                  fill="currentColor"
                />
              </pattern>
            </defs>
            <rect width="404" height="384" fill="url(#de316486-4a29-4312-bdfc-fbce2132a2c1)" />
          </svg>
        </div>
        <div class="grid-col-1">
          <div class="bg-white mt-4 mb-8 rounded-lg overflow-hidden lg:w-3/5">
            <div class="text-base max-w-prose lg:max-w-none">
              <p class="text-lg text-gray-500">
                Regular Talk Speakers
              </p>
            </div>
            <div class="max-w-7xl mx-auto py-12 px-4 text-center sm:px-6 lg:px-8 lg:py-24">
              <div class="space-y-8 sm:space-y-12">
                <ul role="list" class="mx-auto grid grid-cols-2 gap-x-4 gap-y-8 sm:grid-cols-4 md:gap-x-6 lg:max-w-5xl lg:gap-x-8 lg:gap-y-12 xl:grid-cols-5">
                  <li v-for="person in people" :key="person.name">
                    <div class="space-y-4">
                      <img class="mx-auto h-20 w-20 rounded-full lg:w-24 lg:h-24 object-fill" :src="person.imageUrl" alt="">
                      <div class="space-y-2">
                        <div class="text-xs font-medium lg:text-sm">
                          <h3>{{ person.name }}</h3>
                          <p class="text-indigo-600">
                            {{ person.talk_title }}
                          </p>
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      people: [
        {
          name: 'Arie Wahyu Wijayanto',
          nickname: 'Arie',
          role: 'Politeknik Statistika STIS; Lecturer',
          bio: 'A lecturer and Acting Head of Statistical Computing Study Center, Politeknik Statistika STIS. Passionate in machine learning, big data, and remote sensing.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/01%20Arie%20Wahyu%20Wijayanto.JPG',
          talk_title: 'Python for Government Institution: Producing Better Official Statistics',
          twitter: 'https://twitter.com/ariewahyuw',
          github: 'https://github.com/ariewahyu',
          linkedin: 'https://www.linkedin.com/in/ariewahyu/',
          instagram: 'https://www.instagram.com/ariewahyu_',
          youtube: 'https://www.youtube.com/channel/UCfZbGc616UA1gsuFbYgMMCg'
        },
        {
          name: 'Abdurrachman Mappuji',
          nickname: 'mpj',
          role: 'Tech Lead @Mekari',
          bio: 'I\'m an engineer by training and an educator at heart. After graduating from Universitas Gadjah Mada\'s Engineering Physics Program, I started a career in software engineering and worked in various organizations, small and large, startups and corporate. Currently, I\'m exploring metaverse and would like to invite you to join me in the journey. If I\'m not working, you can find me reading books with my Kindle or mentoring the next generation of software engineers.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/02%20Abdurrachman%20Mappuji.png',
          talk_title: 'Blockchain 101: Deploy your first smart contract with Python',
          twitter: 'https://twitter.com/YoKulGuy',
          github: 'https://github.com/empeje',
          linkedin: 'https://www.linkedin.com/in/abmap/',
          instagram: 'https://instagram.com/YoKulGuy/',
          youtube: 'https://www.youtube.com/channel/UCHxI3i2iobjq226ze-N-QBA'
        },
        {
          name: 'Radical Rakhman Wahid',
          nickname: 'Ikal',
          role: 'Data Scientist at Widya Analytic',
          bio: 'Experienced in Python for research and production purposes. Currently working as a Data Scientist at Widya Analytic, Special Region of Yogyakarta, Indonesia.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/03 Radical Rakhman Wahid.jpg',
          talk_title: 'Fooling Your Deep Neural Networks with Torchattacks',
          twitter: '',
          github: 'https://github.com/rakhid16',
          linkedin: 'https://www.linkedin.com/in/rakhid16/',
          instagram: 'https://www.instagram.com/rakhid16/',
          youtube: ''
        },
        {
          name: 'Aria Suseno',
          nickname: 'Uno',
          role: 'Test Engineer & Founder Pyauto ID',
          bio: 'A Software Tester. Build Youtube channel (Ide Jongkok), related to Automation with Python. Founder of PyAuto ID. Speaker & Mentor in Coding ID & Orang Siber.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/04%20Aria%20Suseno.jpg',
          talk_title: 'Headless Web UI Automation Test with Python & Google Colab',
          twitter: '',
          github: '',
          linkedin: 'https://www.linkedin.com/in/aria-uno-suseno/',
          instagram: 'https://www.instagram.com/idejongkok/',
          youtube: 'https://www.youtube.com/c/IdeJongkok/'
        },
        {
          name: 'Hendri Karisma',
          nickname: 'Hendri',
          role: 'Blibli.com; Principal R&D Engineer',
          bio: 'R&D Engineer for Ai & DevEx squad at blibli.com | owner Nevada Kitchen',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/05%20Hendri%20Kharisma.jpg',
          talk_title: 'Managing Config in Python using Consul and Vault',
          twitter: 'infoHendri',
          github: 'situkangsayur',
          linkedin: 'https://www.linkedin.com/in/hendri-karisma-736a0a39/',
          instagram: '',
          youtube: 'situkangsayur'
        },
        {
          name: 'Ali Akbar Septiandri',
          nickname: 'Ali',
          role: 'Revolut; Data scientist',
          bio: 'Learning/teaching data science, machine learning, and artificial intelligence. Host of Tentang Data podcast.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/06%20Ali%20Akbar%20Septiandri.jpg',
          talk_title: 'Learning Reinforcement Learning with OpenAI Gym',
          twitter: 'https://twitter.com/aliakbars',
          github: 'https://github.com/aliakbars/',
          linkedin: 'https://www.linkedin.com/in/aaseptiandri/',
          instagram: 'https://www.instagram.com/aliakbars/',
          youtube: 'https://www.youtube.com/c/AliAkbarSeptiandriID'
        },
        {
          name: 'Harshdeep Singh',
          nickname: 'Harsh',
          role: 'PhD Student, Indian Institute of Technology, Kharagpur',
          bio: 'I am a first-year Ph.D. student and my area of research is quantum computation, and applications of variational quantum algorithms in various fields, etc.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/07%20Harshdeep%20Singh.jpg',
          talk_title: 'Introduction to Quantum Computation using Qiskit',
          twitter: '@harshdeeps3',
          github: '',
          linkedin: 'https://www.linkedin.com/in/harshdeepsingh3/',
          instagram: 'https://www.instagram.com/_harshdeep3/',
          youtube: ''
        },
        {
          name: 'Kemal Maulana Kurniawan',
          nickname: 'Kemal',
          role: 'University of Melbourne; PhD candidate',
          bio: 'Kemal adalah kandidat doktor di University of Melbourne, Australia, dengan bidang keahlian pengolahan bahasa manusia (NLP) dan penggemar bahasa Python.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/08%20Kemal%20Maulana%20Kurniawan.jpg',
          talk_title: 'Implementasi Teorema Matriks-Pohon dengan PyTorch',
          twitter: '@kmkurn',
          github: 'https://github.com/kmkurn',
          linkedin: 'https://www.linkedin.com/in/kemalkurniawan/',
          instagram: '',
          youtube: ''
        },
        {
          name: 'Nicolas Fränkel',
          nickname: 'Nicolas',
          role: 'Hazelcast',
          bio: 'A Java Geek :-)',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/09%20Nicolas%20Fr%C3%A4nkel.jpg',
          talk_title: 'A Guided Tour of Caching Patterns',
          twitter: 'https://twitter.com/nicolas_frankel',
          github: 'https://github.com/nfrankel',
          linkedin: '',
          instagram: '',
          youtube: 'https://www.youtube.com/channel/UC5wHWZfEjZChkgVzg2jnbhQ'
        },
        {
          name: 'Yahya Fadhluloh AlFatih',
          nickname: 'yahya',
          role: 'Cyber Security Researcher',
          bio: 'oss enthusiast and Computerphile',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/10%20Yahya%20Fadhluloh%20AlFatih.jpg',
          talk_title: 'The Importance of Python for Ethical Hacking',
          twitter: 'https://twitter.com/BukanYahya',
          github: 'https://github.com/k1m0ch1',
          linkedin: 'www.linkedin.com/in/yahya-fadhlulloh-al-fatih-a568a455',
          instagram: '',
          youtube: 'https://www.youtube.com/c/k1m0ch1'
        },
        {
          name: 'Merve Noyan',
          nickname: 'Merve',
          role: 'Hugging Face',
          bio: 'Developer Advocate at Hugging Face, Google Developer Expert in Machine Learning',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/11%20Merve%20Noyan.png',
          talk_title: 'Building Machine Learning Demos using Python',
          twitter: 'mervenoyann',
          github: 'merveenoyan',
          linkedin: 'https://www.linkedin.com/in/merve-noyan-28b1a113a/',
          instagram: '',
          youtube: ''
        },
        {
          name: 'Andi Dinata',
          nickname: 'Andi',
          role: 'Colab Coding',
          bio: 'Published Author who teach Coding Class and DIY electronic enthusiast',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/12%20Andi%20Dinata.png',
          talk_title: 'Unfold Python Secrets to Student',
          twitter: 'https://twitter.com/mcdinata',
          github: 'github.com/mdinata',
          linkedin: 'https://www.linkedin.com/in/andi-dinata-061368102',
          instagram: 'https://www.instagram.com/mdinata/',
          youtube: ''
        },
        {
          name: 'Mahmud Isnan',
          nickname: 'Mahmud',
          role: 'SIIT, Thammasat University',
          bio: 'I am a master student in the field of AI and IOT in SIIT, Thammasat University, Thailand. I work in remote sensing and machine learning.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/13%20Mahmud%20Isnan.jpg',
          talk_title: 'Python for land monitoring Using Geemap',
          twitter: '',
          github: '',
          linkedin: 'https://www.linkedin.com/in/mahmud-isnan-537377145/',
          instagram: 'https://www.instagram.com/mahmudisnan18/',
          youtube: ''
        },
        {
          name: 'Karan Balkar',
          nickname: 'Karan',
          role: 'Team Lead',
          bio: 'Karan Balkar is a mobile application developer primarily working on Android since the past 5 years. He has also worked on Augmented reality / Virtual reality based mobile applications and is passionate about exploring new innovative technologies.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/14%20Karan%20Balkar.png',
          talk_title: 'Using Chaos toolkit to determine resiliency for your web app',
          twitter: '',
          github: '',
          linkedin: '',
          instagram: 'https://www.instagram.com/karanbalkar/?hl=en',
          youtube: ''
        },
        {
          name: 'Harsh Bardhan Mishra',
          nickname: 'Harsh',
          role: 'Quansight Labs',
          bio: 'Harsh is a Software Developer at Quansight Labs and Google Summer of Code Student developer at MetaCall. His interest lies in DevOps, Docs and Web engineering.',
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/15%20Harsh%20Bardhan%20Mishra.jpeg',
          talk_title: 'Build custom wrapper kernels using IPython',
          twitter: 'https://twitter.com/harsh_casper',
          github: 'https://github.com/harshcasper',
          linkedin: 'https://www.linkedin.com/in/harshcasper',
          instagram: 'https://www.instagram.com/harshcasper/',
          youtube: ''
        },
        {
          name: 'Ridwan Fadjar Septian',
          nickname: 'Ridwan',
          role: 'Cloud Infrastructure Engineer',
          bio: `
            I am working at NiceDay for years. First time I joined with this company the name was still Sensehealth B.V., I was hired as Backend Developer and using Python3, Django, Celery and Ejabberd to build web services for helping Dutch who need help in for their mental health.

            As NIceDay expanded their market in Netherlands, I was assigned to be Cloud Infrastructure Engineer and involve on bulding infrastructure for better NiceDay web services with Infrastructure Team. This team was established 3 years ago. So, I am focusing to infrastructures more rather than to backend application development.

            As part of this talk, I am working with Prometheus + Alert Manager + OpsGenie, ELK and Sentry to handle any issues that might be happened by our Django Web Application. We are using those tools because we deploy our Django Web Application on Docker and Container Orchestration. So its kind of we have multiple Django servers. So, monitoring and logging system should be centralized in single environment.
          `,
          imageUrl: 'https://ik.imagekit.io/9rpt33mvmla/tr:h-360,w-360,cm-maintain_ratio/pyconid2021/speakers/16%20Ridwan%20Fadjar%20Septian.jpg',
          talk_title: 'Monitoring and Logging Django Web Application with Prometheus, ELK and Sentry',
          twitter: '',
          github: 'https://github.com/ridwanbejo/',
          linkedin: 'https://www.linkedin.com/in/ridwan-fadjar-79781756/',
          instagram: '',
          youtube: ''
        }
      ]
    }
  }
}
</script>
