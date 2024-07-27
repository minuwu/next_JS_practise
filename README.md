## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.


/layout.tsx
import '@/app/ui/global.css';

/home.module.css
.shape {
    height: 0;
    width: 0;
    border-bottom: 30px solid black;
    border-left: 20px solid transparent;
    border-right: 20px solid transparent;
}

/page.tsx
import styles from '@/app/ui/home.module.css';
<div className={styles.shape}/>

/fonts.ts
import { Inter } from 'next/font/google';
export const inter = Inter({ subsets: ['latin']});

/layout.tsx
import { inter } from '@/app/ui/fonts';
<body className={`${inter.className} antialiased`} >{children}</body>

/page.ts
<Image 
    src="/hero-desktop.png" 
    width={1000} 
    height={760} 
    className="hidden md:block" 
    alt='Screenshots of the dashboard project showing desktop version'
/>
<Image
    src="/hero-mobile.png"
    width={560}
    height={620}
    className='block md:hidden'
    alt='Screenshots of the dashboard project showing mobile version'
/>