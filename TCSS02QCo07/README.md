## Tailwind CSS 02
## Chapter 2: Project Header, Hero & Cards
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 Tailwind CSS 資源
https://github.com/gitdagray/tailwind-css-course

### Dave Gray 的 Tailwind CSS 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6M8znNpim8dRiICRrP5HPft&si=TYz4MlVwoMJZuO69

### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## Quick Concept offline
###  1. Intro
        教學影片開頭和介紹

###  2. Welcome

###  3. Project Preview

###  4. Project Setup
        (1)在 terminal 輸入 npx tailwindcss init
        (2)新增資料夾 build
        (3)新增資料夾 src
        (4)新增 input.css
        (5)新增 base
        (6)新增 components
        (7)新增 utilities
        (8)新增 index.html
        (9)新增資料夾 img
        (10)新增 rocketride.png, rocketman.png, rocketlaunch.png, rocketdab.png
        (11)新增 favicon.ico
        (12)加入 html 路徑為 ./build/*.html
        (13)在 terminal 輸入 npm init -y
        (14)在 package.json 的 scripts，
        設定 tailwind，指令為 npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch
        (15)在 terminal 輸入 npm i -D prettier-plugin-tailwindcss
        (16)新增 .gitignore，輸入 node_modules
        (17)在 package.json 的 scripts，
        設定 prettier，指令為 npx prettier --write **/*.html
        (18)在 terminal 輸入 npm run tailwind
        即在 terminal 執行 npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch

###  5. Starting the Website
        (1)輸入!，使用 Emmet Abbreviation
        (2)修改 title元素文字為 Acme Rockets
        (3)加入 style.css 於 index.html
        (4)設定 body 元素的 Class
        新增 min-h-screen 為 min-height: 100vh;
        新增 bg-slate-50 為 background-color: rgb(255 255 255);
        在深色模式中，
        新增 bg-black 為 background-color: rgb(0 0 0);
        新增 text-white 為 color: rgb(255 255 255);

###  6. header and nav styles
        (1)設定 header 元素的 Class
        新增 bg-teal-700 為 background-color: rgb(15 118 110);
        新增 text-white 為 color: rgb(255 255 255);
        新增 sticky 為 position: sticky;
        新增 top-0 為 top: 0px;
        新增 z-10 為 z-index: 10;

        (2)設定 section 元素的 Class
        新增 max-w-4xl 為 max-width: 56rem; /* 896px */
        新增 mx-auto 為 margin-left: auto; margin-right: auto;
        新增 p-4 為 padding: 1rem
        新增 flex 為 display: flex
        新增 justify-between 為 justify-content: space-between
        新增 items-center 為 align-items: center

        (3)設定 h1 元素的 Class
        新增 text-3xl 為 
        font-size: 1.875rem; /* 30px */
        line-height: 2.25rem; /* 36px */
        新增 font-medium 為 font-weight: 500;
        設定 h1 元素的文字為 Acme Rockets

        (4)設定 a 元素的超連結為 #hero，文字為 Acme Rockets
        (5)新增 div元素

        (6)新增 button元素，id 為 mobile-open-button
        設定 button元素的 Class
        新增 text-3xl 為 
        font-size: 1.875rem; /* 30px */
        line-height: 2.25rem; /* 36px */
        新增 sm:hidden 為 
        @media (min-width: 640px) {
                display: none;
        }
        新增 focus:outline-none 為 
        button:focus {
                outline: 2px solid transparent;
                outline-offset: 2px;
        }
        設定 button元素的選單圖示

        (7)設定 nav元素的 Class
        新增 hidden 為 display: none;
        新增 sm:block 為 
        @media (min-width: 640px) {
                display: block
        }
        新增 space-x-8 為 margin-left: 2rem;
        新增 text-xl 為 
        font-size: 1.25rem; /* 20px */
        line-height: 1.75rem; /* 28px */
        設定 nav元素的 aria-label 為 main

        (8)新增 a 元素的超連結為 #rockets，
        設定 a 元素的 Class
        新增 hover:opacity-90 為 a:hover { opacity: 0.9; }
        文字為 Our Rockets
        (9)新增 a 元素的超連結為 #testimonials，
        文字為 Testimonials
        (10)新增 a 元素的超連結為 #contact，
        文字為 Contact Us

###  7. Hero section
        (1)設定 main元素的 Class
        新增 max-w-4xl 為 max-width: 56rem; /* 896px */
        新增 mx-auto 為 margin-left: auto; margin-right: auto;

        (2)設定 section元素的 Class
        新增 flex 為 display: flex;
        新增 flex-col-reverse 為 flex-direction: column-reverse;
        新增 justify-center 為 justify-content: center;
        新增 sm:flex-row 為 
        @media (min-width: 640px) {
                display: none;
        }
        新增 p-6 為 padding: 1.5rem; /* 24px */
        新增 items-center 為 align-items: center;
        新增 gap-8 為 column-gap: 2rem; /* 32px */
        新增 mb-12 為 margin-bottom: 3rem; /* 48px */

        (3)設定 article元素的 Class，
        新增 sm:w-1/2 為 
        @media (min-width: 640px) {
                width: 50%;
        }

        (4)設定 h2元素的 Class，
        新增 max-w-md 為 max-width: 28rem; /* 448px */
        新增 text-4xl 為 
        font-size: 2.25rem; /* 36px */
        line-height: 2.5rem; /* 40px */
        新增 font-bold 為 font-weight: bold
        新增 text-center 為 text-align: center;
        新增 sm:text-5xl 為 
        @media (min-width: 640px) { 
                font-size: 3rem; /* 48px */
                line-height: 1;
        }
        新增 sm:text-left 為 
        @media (min-width: 640px) {
                text-align: left;
        }
        新增 text-slate-900 為 color: rgb(15 23 42);
        新增 dark:text-white 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(255 255 255);
        }
        文字為 We Boldy Go Where No Rocket Has Gone Before...

        (5)設定 span元素的 Class，
        新增 text-indigo-700 為 color: rgb(67 56 202);
        新增 dark:text-indigo-300 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(255 255 255);
        }
        文字為 Where No Rocket

        (6)設定 p元素的 Class，
        文字為 We are building rockets for the next century today. From the moon to Mars, Jupiter and beyond...

        (7)設定 p元素的 Class，
        文字為 Think Acme Rockets.

        (8)設定 img元素的 Class，
        新增 max-w-md 為 max-width: 28rem; /* 448px */
        路徑為 ./img/rocketdab.png
        圖片替代文字為 rocketdab

###  8. horizontal rule
        設定 hr元素的 Class，
        新增 mx-auto 為 margin-left: auto; margin-right: auto;
        新增 bg-black 為 background-color: rgb(0 0 0);
        新增 dark:bg-white 為
        @media (prefers-color-scheme: dark) {
                background-color: rgb(255 255 255);
        }
        新增 w-1/2 為 width: 50%;

###  9. Rockets section
        (1)設定 section元素的 id 為 rockets，
        設定 section元素的 Class，
        新增 p-6 為 padding: 1.5rem; /* 24px */
        新增 my-12 為
        margin-top: 3rem; /* 48px */
        margin-bottom: 3rem; /* 48px */

        (2)設定 h2元素的 Class，
        新增 text-4xl 為 
        font-size: 2.25rem; /* 36px */
        line-height: 2.5rem; /* 40px */
        新增 font-bold 為 font-weight: bold
        新增 text-center 為 text-align: center;
        新增 sm:text-5xl 為 
        @media (min-width: 640px) { 
                font-size: 3rem; /* 48px */
                line-height: 1;
        }
        新增 mb-6 為 margin-bottom: 1.5rem; /* 24px */
        新增 text-slate-900 為 color: rgb(15 23 42);
        新增 dark:text-white 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(255 255 255);
        }
        文字為 Our Rockets

        (3)設定 hr元素
        設定 section元素，id 為 testimonials

        設定 section元素的 Class，
        新增 p-6 為 padding: 1.5rem; /* 24px */
        新增 my-12 為
        margin-top: 3rem; /* 48px */
        margin-bottom: 3rem; /* 48px */
        新增 scroll-mt-20 為 scroll-margin-top: 5rem; /* 80px */
        設定 h2元素，文字為 Testimonials

        (4)設定 hr元素
        設定 section元素，id 為 contact
        設定 section元素的 Class，
        新增 p-6 為 padding: 1.5rem; /* 24px */
        新增 my-12 為
        margin-top: 3rem; /* 48px */
        margin-bottom: 3rem; /* 48px */
        設定 h2元素，文字為 Contact Us

        (5)在 id 為 rockets 的 section元素 加入
        設定 ul元素的 Class，
        新增 list-none 為 list-style-type: none;
        新增 mx-auto 為 margin-left: auto; margin-right: auto;
        新增 my-12 為
        margin-top: 3rem; /* 48px */
        margin-bottom: 3rem; /* 48px */
        新增 flex 為 display: flex;
        新增 flex-col 為 flex-direction: column;
        新增 sm:flex-row 為 
        @media (min-width: 640px) {
                flex-direction: row;
        }
        新增 items-center 為 align-items: center;
        新增 gap-8 為 column-gap: 2rem; /* 32px */

        (6)設定 li元素的 Class，
        新增 w-2/3 為 width: 66.666667%;
        新增 sm:w-5/6 為 
        @media (min-width: 640px) {
                width: 83.333333%;
        }
        新增 flex 為 display: flex;
        新增 flex-col 為 flex-direction: column;
        新增 items-center 為 align-items: center;

        新增 border 為
        新增 border-solid 為 border-style: solid;
        新增 border-slate-900 為 border-color: rgb(15 23 42);
        新增 dark:border-gray-100 為
        @media (prefers-color-scheme: dark) {
                color: rgb(255 255 255);
        }
        新增 bg-white 為 background-color: rgb(255 255 255);
        新增 dark:bg-black 為 
        @media (prefers-color-scheme: dark) {
                background-color: rgb(0 0 0);
        }
        新增 py-6 為
        padding-top: 1.5rem; /* 24px */
        padding-bottom: 1.5rem; /* 24px */

        新增 px-2 為
        padding-left: 0.5rem; /* 8px */
        padding-right: 0.5rem; /* 8px */

        新增 rounded-3xl 為 border-radius: 1.5rem; /* 24px */
        新增 shadow-xl 為
        box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);

        (7)設定 img元素的 Class，
        新增 w-1/2 為 width: 50%;
        新增 mb-6 為 margin-bottom: 1.5rem; /* 24px */
        路徑為 ./img/rocketman.png
        圖片替代文字為 Explorer

        (8)設定 h3元素的 Class，
        新增 text-3xl 為 
        font-size: 1.875rem; /* 30px */
        line-height: 2.25rem; /* 36px */

        新增 text-center 為 text-align: center;

        新增 text-slate-900 為 color: rgb(15 23 42);
        新增 dark:text-white 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(255 255 255);
        }
        文字為 Explorer

        (9)設定 p元素的 Class，
        新增 hidden 為 display: none;
        新增 sm:block 為 
        @media (min-width: 640px) { display: block }
        新增 text-3xl 為 
        font-size: 1.875rem; /* 30px */
        line-height: 2.25rem; /* 36px */

        新增 text-center 為 text-align: center;
        新增 mt-2 為 margin-top: 0.5rem; /* 8px */
        新增 text-slate-500 為 color: rgb(100 116 139);
        新增 dark:text-slate-400 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(148 163 184);
        }
        文字為 $

        (10)設定 p元素的 Class，
        新增 sm:hidden 為 
        @media (min-width: 640px) { display: none; }
        新增 text-2xl 為 
        font-size: 1.5rem; /* 24px */
        line-height: 2rem; /* 32px */
        新增 text-center 為 text-align: center;
        新增 mt-2 為 margin-top: 0.5rem; /* 8px */
        新增 text-slate-500 為 color: rgb(100 116 139);
        新增 dark:text-slate-400 為 
        @media (prefers-color-scheme: dark) {
                color: rgb(148 163 184);
        }
        文字為 Affordable Exploreration

        (11)設定 li元素，
        設定 img元素，
        路徑為 ./img/rocketride.png
        圖片替代文字為 Adventurer
        設定 h3元素，文字為 Adventurer
        設定第一個 p元素，文字為 $$
        設定第二個 p元素，文字為 Best Selling Rocket!

        (12)設定 li元素，
        設定 img元素，
        路徑為 ./img/rocketlaunch.png
        圖片替代文字為 Infinity
        設定 h3元素，文字為 Infinity
        設定第一個 p元素，文字為 $$$
        設定第二個 p元素，文字為 Luxury Starship

### 10. Scroll settings
        (1)在 id 為 hero 的 section元素，
        修改 section元素的 Class 為
        flex flex-col-reverse justify-center sm:flex-row p-6 items-center gap-8 mb-12 scroll-mt-40
        scroll-mt-40 為 scroll-margin-top: 10rem; /* 160px */

        (2)在 id 為 rockets 的 section元素，
        修改 section元素的 Class 為 p-6 my-12 scroll-mt-20
        scroll-mt-20 為 scroll-margin-top: 5rem; /* 80px */

        (3)在 id 為 testimonials 的 section元素，
        修改 section元素的 Class 為 p-6 my-12 scroll-mt-20
        新增 scroll-mt-20 為 scroll-margin-top: 5rem; /* 80px */

        (4)在 id 為 contact 的 section元素，
        修改 section元素的 Class 為 p-6 my-12 scroll-mt-16
        scroll-mt-16 為 scroll-margin-top: 4rem; /* 64px */

        (5)設定 html元素的 Class，
        新增 sm:scroll-smooth 為
        @media (min-width: 640px) {
                scroll-behavior: smooth;
        }