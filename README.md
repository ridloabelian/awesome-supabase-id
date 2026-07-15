<div align="center">

<img src="https://raw.githubusercontent.com/supabase/supabase/master/packages/common/assets/images/supabase-logo-wordmark--dark.svg" alt="Supabase Logo" width="300" />

<h1 align="center">Kitab Supabase ⚡️ 🇮🇩<br><sub>(Stack Nol Rupiah)</sub></h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=3ECF8E&center=true&vCenter=true&width=600&lines=Postgres+Gratis+Selamanya;Auth+%2B+Realtime+%2B+Storage;Firebase+Alternative+Open-Source;Bangun+SaaS+Modal+Rp+0" alt="Typing SVG" />
</p>

Kumpulan *boilerplate*, *starter kit*, template, dan proyek *open-source* terbaik berbasis **Supabase** — platform *backend* open-source (Postgres, Auth, Storage, Realtime, Edge Functions) yang jadi alternatif Firebase.
Dibangun untuk membantu developer & *indie hacker* Indonesia meluncurkan produk SaaS dengan *backend* profesional bermodal Rp 0.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Stars](https://img.shields.io/github/stars/ridloabelian/awesome-supabase-id?style=flat&color=3ECF8E)](https://github.com/ridloabelian/awesome-supabase-id/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/ridloabelian/awesome-supabase-id?style=flat&color=3ECF8E)](https://github.com/ridloabelian/awesome-supabase-id/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](LICENSE)

</div>

> 🗺️ **Bagian dari seri [Stack Nol Rupiah](https://github.com/ridloabelian/awesome-rp0-id)** — peta lengkap bootstrap gratisan Rp 0 untuk indie hacker Indonesia.

> 🔗 **Repo saudara:** Lihat juga [**Kitab Cloudflare**](https://github.com/ridloabelian/awesome-cloudflare-id) (edge/serverless) dan [**Kitab Google**](https://github.com/ridloabelian/awesome-google-free-id) (automasi bisnis). **Kombinasi paling sakti: Cloudflare (frontend/edge) + Supabase (database/auth) = stack SaaS Rp 0 paling populer di kalangan indie hacker.**

Supabase memberikan yang tidak dimiliki Firebase: **database SQL sungguhan (PostgreSQL)**. Anda dapat Auth, Storage, Realtime subscription, Edge Functions, dan Vector (pgvector untuk AI) — semuanya open-source dan bisa di-*self-host* jika perlu. Free tier-nya sangat cukup untuk memvalidasi ide sampai mendapat pengguna pertama.

**Kriteria Kurasi:**
- Berjalan atau berbasis Supabase (cloud free tier atau self-hosted).
- Mempercepat *development* SaaS, aplikasi web, atau mobile.
- *Open-source* dan idealnya masih aktif di-*maintain*.
- Bermanfaat untuk konteks solopreneur & developer Indonesia.

---

## 💰 Batas Gratis (Free Tier) Supabase

Acuan umum paket **Free** Supabase. Selalu cek [halaman pricing](https://supabase.com/pricing) karena kebijakan bisa berubah.

| Fitur | Batas Gratis | Catatan |
|-------|--------------|---------|
| **Database (Postgres)** | 500 MB | Database SQL penuh, bukan sekadar key-value. |
| **Auth (MAU)** | 50.000 *Monthly Active Users* | Sangat besar untuk fase awal. Login email, OAuth, magic link. |
| **Storage** | 1 GB | Penyimpanan file + CDN. |
| **Bandwidth** | 5 GB/bulan | Transfer data keluar. |
| **Edge Functions** | 500.000 invokasi/bulan | Serverless Deno untuk logika backend. |
| **Realtime** | 200 koneksi bersamaan, 2 juta pesan/bln | WebSocket untuk fitur live/kolaborasi. |
| **Vector (pgvector)** | Termasuk dalam DB | Untuk aplikasi AI/RAG & pencarian semantik. |

> ⚠️ **Penting:** Proyek gratis akan **di-*pause* otomatis setelah 1 minggu tidak aktif** (bisa di-restore). Batas 2 proyek aktif untuk akun gratis. Untuk produksi serius, paket Pro mulai $25/bln — tapi untuk validasi & MVP, free tier sudah lebih dari cukup.

---

## Daftar Isi
- [💰 Batas Gratis (Free Tier) Supabase](#-batas-gratis-free-tier-supabase)
- [🛠️ Tooling Resmi & CLI](#️-tooling-resmi--cli)
- [🚀 SaaS Boilerplate (Next.js)](#-saas-boilerplate-nextjs)
- [🎨 SaaS Boilerplate (Svelte/Nuxt/Lainnya)](#-saas-boilerplate-sveltenuxtlainnya)
- [🔐 Auth & SSR Template](#-auth--ssr-template)
- [💬 Realtime & Chat](#-realtime--chat)
- [⚡ Supabase + Cloudflare (Edge)](#-supabase--cloudflare-edge)
- [📱 Mobile (Flutter)](#-mobile-flutter)
- [🤖 AI & Micro-SaaS](#-ai--micro-saas)
- [📊 Admin Dashboard](#-admin-dashboard)
- [📚 Referensi](#-referensi)
- [📄 Template Siap Pakai](#-template-siap-pakai)

---

## 🛠️ Tooling Resmi & CLI
Alat resmi dari tim Supabase untuk development, migrasi, dan deploy.

| Nama | Deskripsi |
|------|-----------|
| [supabase/cli](https://github.com/supabase/cli) ![](https://img.shields.io/github/stars/supabase/cli?style=flat&label=%E2%98%85&color=3ECF8E) | CLI resmi Supabase. Jalankan Supabase secara lokal (Docker), kelola migrasi Postgres, dan deploy Edge Functions. |
| [supabase/supabase-js](https://github.com/supabase/supabase-js) ![](https://img.shields.io/github/stars/supabase/supabase-js?style=flat&label=%E2%98%85&color=3ECF8E) | Klien JavaScript isomorphic. Query database, subscribe realtime, auth, dan storage dari browser maupun Node. |
| [supabase/supabase-py](https://github.com/supabase/supabase-py) ![](https://img.shields.io/github/stars/supabase/supabase-py?style=flat&label=%E2%98%85&color=3ECF8E) | Klien Python resmi. Query Postgres dari Flask, Django, atau FastAPI. |

## 🚀 SaaS Boilerplate (Next.js)
Kerangka SaaS siap pakai berbasis React/Next.js — tinggal fokus ke bisnis Anda.

| Nama | Deskripsi |
|------|-----------|
| [imbhargav5/nextbase-nextjs-supabase-starter](https://github.com/imbhargav5/nextbase-nextjs-supabase-starter) ![](https://img.shields.io/github/stars/imbhargav5/nextbase-nextjs-supabase-starter?style=flat&label=%E2%98%85&color=3ECF8E) | Boilerplate gratis & lengkap untuk Next.js 16+, Supabase, Tailwind CSS 4, dan TypeScript. |
| [makerkit/nextjs-saas-starter-kit-lite](https://github.com/makerkit/nextjs-saas-starter-kit-lite) ![](https://img.shields.io/github/stars/makerkit/nextjs-saas-starter-kit-lite?style=flat&label=%E2%98%85&color=3ECF8E) | Versi *lite* dari Makerkit SaaS Starter Kit berbasis Next.js dan Supabase. Populer & terawat. |
| [antoineross/Hikari](https://github.com/antoineross/Hikari) ![](https://img.shields.io/github/stars/antoineross/Hikari?style=flat&label=%E2%98%85&color=3ECF8E) | Starter SaaS Next.js 14 + Stripe + Supabase yang komplit dan open-source. |
| [michaeltroya/supa-next-starter](https://github.com/michaeltroya/supa-next-starter) ![](https://img.shields.io/github/stars/michaeltroya/supa-next-starter?style=flat&label=%E2%98%85&color=3ECF8E) | Starter Next.js + Supabase + Tailwind + shadcn yang bersih dan modern. |

## 🎨 SaaS Boilerplate (Svelte/Nuxt/Lainnya)
Bukan cuma React — pilihan untuk penggemar Svelte, Vue/Nuxt, dan FastAPI.

| Nama | Deskripsi |
|------|-----------|
| [scosman/CMSaasStarter](https://github.com/scosman/CMSaasStarter) ![](https://img.shields.io/github/stars/scosman/CMSaasStarter?style=flat&label=%E2%98%85&color=3ECF8E) | Template SaaS modern berbasis SvelteKit, Tailwind, dan Supabase. Ringan dan sangat lengkap (paling populer di kelasnya). |
| [JavascriptMick/supanuxt-saas](https://github.com/JavascriptMick/supanuxt-saas) ![](https://img.shields.io/github/stars/JavascriptMick/supanuxt-saas?style=flat&label=%E2%98%85&color=3ECF8E) | Boilerplate SaaS untuk Nuxt 3 + Supabase + OAuth + Prisma + tRPC + Stripe. |
| [AtticusZeller/fastapi_supabase_template](https://github.com/AtticusZeller/fastapi_supabase_template) ![](https://img.shields.io/github/stars/AtticusZeller/fastapi_supabase_template?style=flat&label=%E2%98%85&color=3ECF8E) | Template FastAPI yang terintegrasi dalam dengan Supabase: auth, CRUD Postgres, dan upload file. |

## 🔐 Auth & SSR Template
Fokus pada sistem autentikasi yang aman dengan Server-Side Rendering.

| Nama | Deskripsi |
|------|-----------|
| [ElectricCodeGuy/SupabaseAuthWithSSR](https://github.com/ElectricCodeGuy/SupabaseAuthWithSSR) ![](https://img.shields.io/github/stars/ElectricCodeGuy/SupabaseAuthWithSSR?style=flat&label=%E2%98%85&color=3ECF8E) | Supabase Auth + AI Stack untuk Next.js 15 dengan SSR dan React Server Components (RSC). |
| [jabirdev/nextjs-better-auth](https://github.com/jabirdev/nextjs-better-auth) ![](https://img.shields.io/github/stars/jabirdev/nextjs-better-auth?style=flat&label=%E2%98%85&color=3ECF8E) | Starter Next.js 16 dengan Better Auth, Drizzle ORM, dan Supabase. |
| [engageintellect/sveltekit-supabase](https://github.com/engageintellect/sveltekit-supabase) ![](https://img.shields.io/github/stars/engageintellect/sveltekit-supabase?style=flat&label=%E2%98%85&color=3ECF8E) | Starter minimal Svelte 5 + Supabase + shadcn-svelte dengan login GitHub. |

## 💬 Realtime & Chat
Manfaatkan fitur Realtime Supabase untuk aplikasi chat & kolaborasi live.

| Nama | Deskripsi |
|------|-----------|
| [shwosner/realtime-chat-supabase-react](https://github.com/shwosner/realtime-chat-supabase-react) ![](https://img.shields.io/github/stars/shwosner/realtime-chat-supabase-react?style=flat&label=%E2%98%85&color=3ECF8E) | Aplikasi chat realtime menggunakan React dan Supabase Realtime. |
| [supabase-community/flutter-chat](https://github.com/supabase-community/flutter-chat) ![](https://img.shields.io/github/stars/supabase-community/flutter-chat?style=flat&label=%E2%98%85&color=3ECF8E) | Aplikasi chat sederhana dibuat dengan Flutter dan Supabase (proyek komunitas resmi). |
| [arnu515/supabase-e2ee-chat](https://github.com/arnu515/supabase-e2ee-chat) ![](https://img.shields.io/github/stars/arnu515/supabase-e2ee-chat?style=flat&label=%E2%98%85&color=3ECF8E) | Aplikasi chat dengan enkripsi *end-to-end* berbasis Supabase. |

## ⚡ Supabase + Cloudflare (Edge)
Kombinasi paling powerful: data Supabase disajikan dari edge Cloudflare Workers.

| Nama | Deskripsi |
|------|-----------|
| [supaflare/supaflare](https://github.com/supaflare/supaflare) ![](https://img.shields.io/github/stars/supaflare/supaflare?style=flat&label=%E2%98%85&color=3ECF8E) | Layanan URL shortener/redirect berbasis Supabase + Cloudflare Workers. Contoh integrasi sempurna keduanya. |
| [kristianfreeman/supabase-workers-proxy](https://github.com/kristianfreeman/supabase-workers-proxy) ![](https://img.shields.io/github/stars/kristianfreeman/supabase-workers-proxy?style=flat&label=%E2%98%85&color=3ECF8E) | *Proof-of-concept* melakukan request ke Supabase dari dalam Cloudflare Workers. |
| [dijonmusters/supabase-data-at-the-edge](https://github.com/dijonmusters/supabase-data-at-the-edge) ![](https://img.shields.io/github/stars/dijonmusters/supabase-data-at-the-edge?style=flat&label=%E2%98%85&color=3ECF8E) | Pelajari cara *cache* data Supabase di Edge menggunakan Cloudflare Workers + KV Storage. |

## 📱 Mobile (Flutter)
Bangun aplikasi mobile cross-platform dengan backend Supabase.

| Nama | Deskripsi |
|------|-----------|
| [supabase/supabase-flutter](https://github.com/supabase/supabase-flutter) ![](https://img.shields.io/github/stars/supabase/supabase-flutter?style=flat&label=%E2%98%85&color=3ECF8E) | Integrasi Flutter resmi untuk Supabase. Auth, database, storage, dan realtime untuk aplikasi mobile. |
| [devtodollars/mvp-boilerplate](https://github.com/devtodollars/mvp-boilerplate) ![](https://img.shields.io/github/stars/devtodollars/mvp-boilerplate?style=flat&label=%E2%98%85&color=3ECF8E) | Boilerplate mobile & web yang mencakup semua kebutuhan MVP berbasis Supabase. |
| [dshukertjr/spot](https://github.com/dshukertjr/spot) ![](https://img.shields.io/github/stars/dshukertjr/spot?style=flat&label=%E2%98%85&color=3ECF8E) | Aplikasi sosial berbagi video berbasis geolokasi, open-source, dibuat dengan Flutter dan Supabase. |

## 🤖 AI & Micro-SaaS
Bangun aplikasi AI (RAG, chatbot) memanfaatkan pgvector Supabase.

| Nama | Deskripsi |
|------|-----------|
| [emarco177/dandi](https://github.com/emarco177/dandi) ![](https://img.shields.io/github/stars/emarco177/dandi?style=flat&label=%E2%98%85&color=3ECF8E) | Boilerplate untuk membangun micro-SaaS bertenaga AI dengan Next.js, LangChain JS, dan Supabase. |
| [akdeb/ElatoAI](https://github.com/akdeb/ElatoAI) ![](https://img.shields.io/github/stars/akdeb/ElatoAI?style=flat&label=%E2%98%85&color=3ECF8E) | Voice AI realtime dengan 100+ model di Arduino ESP32 menggunakan Secure Websockets dan Supabase Edge Functions. |

## 📊 Admin Dashboard
Panel admin siap pakai untuk mengelola data Supabase Anda.

| Nama | Deskripsi |
|------|-----------|
| [taiwo-adewale/ecommerce-admin](https://github.com/taiwo-adewale/ecommerce-admin) ![](https://img.shields.io/github/stars/taiwo-adewale/ecommerce-admin?style=flat&label=%E2%98%85&color=3ECF8E) | Dashboard admin e-commerce dengan Next.js, shadcn ui, React Query, dan Supabase. |
| [EkiZR/Portofolio_V5](https://github.com/EkiZR/Portofolio_V5) ![](https://img.shields.io/github/stars/EkiZR/Portofolio_V5?style=flat&label=%E2%98%85&color=3ECF8E) | Portfolio pribadi React + Supabase, dilengkapi dashboard admin untuk kelola konten. |

## 📚 Referensi
Sumber belajar dan awesome-list resmi.

| Nama | Deskripsi |
|------|-----------|
| [lyqht/awesome-supabase](https://github.com/lyqht/awesome-supabase) ![](https://img.shields.io/github/stars/lyqht/awesome-supabase?style=flat&label=%E2%98%85&color=3ECF8E) | *Awesome-list* resmi (berbahasa Inggris) berisi starter & sumber daya Supabase. Rujukan utama. |
| [dmotz/trystero](https://github.com/dmotz/trystero) ![](https://img.shields.io/github/stars/dmotz/trystero?style=flat&label=%E2%98%85&color=3ECF8E) | Bonus: bangun webapp multiplayer instan tanpa server (WebRTC). Pelengkap bagus untuk fitur realtime. |

## 📄 Template Siap Pakai
Cuplikan siap pakai untuk pola paling umum. Jalankan SQL di **SQL Editor** dashboard Supabase, dan JS di aplikasi Anda.

### 1. Setup Tabel + Row Level Security (RLS) Wajib
```sql
-- Buat tabel + aktifkan RLS (WAJIB, ini yang sering dilupakan pemula = data bocor!)
create table todos (
  id uuid primary key default gen_random_uuid(),
  user_id uuid references auth.users default auth.uid(),
  task text not null,
  is_done boolean default false,
  created_at timestamptz default now()
);

alter table todos enable row level security;

-- Kebijakan: user hanya bisa akses datanya sendiri
create policy "user kelola todo sendiri" on todos
  for all using (auth.uid() = user_id);
```

### 2. Auth + Query dari JavaScript (supabase-js)
```javascript
import { createClient } from '@supabase/supabase-js';

const supabase = createClient(
  'https://xxxx.supabase.co',        // Project URL
  'PUBLIC_ANON_KEY'                  // Anon key (aman untuk client, dilindungi RLS)
);

// Login via magic link (tanpa password)
await supabase.auth.signInWithOtp({ email: 'user@email.com' });

// Insert data (user_id otomatis dari auth.uid() berkat default di tabel)
await supabase.from('todos').insert({ task: 'Belajar Supabase' });

// Query data (RLS otomatis memfilter hanya milik user login)
const { data } = await supabase.from('todos').select('*').order('created_at');
```

### 3. Realtime Subscription (Live Update)
```javascript
// Dengarkan perubahan tabel secara realtime tanpa polling
supabase
  .channel('todos-realtime')
  .on('postgres_changes',
    { event: '*', schema: 'public', table: 'todos' },
    (payload) => console.log('Perubahan:', payload)
  )
  .subscribe();
```

### 4. Query dari Cloudflare Workers (Kombinasi Sakti)
```javascript
// Di Cloudflare Worker — Supabase sebagai database, Worker sebagai edge API
import { createClient } from '@supabase/supabase-js';

export default {
  async fetch(request, env) {
    const supabase = createClient(env.SUPABASE_URL, env.SUPABASE_ANON_KEY);
    const { data, error } = await supabase.from('todos').select('*').limit(10);
    return Response.json(error ? { error } : { data });
  }
};
```

---

## 🤝 Kontribusi
Jika Anda menemukan *tools* menarik lainnya atau sedang membangun *side project* berbasis Supabase, silakan buat *Pull Request*! Baca dulu [panduan kontribusi](CONTRIBUTING.md) kami.

<a href="https://github.com/ridloabelian/awesome-supabase-id/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ridloabelian/awesome-supabase-id" alt="Contributors" />
</a>

## 📜 Lisensi
Lisensi MIT - [Ridlo Abelian](https://github.com/ridloabelian)

---

<div align="center">

<a href="#kitab-supabase--">⬆️ Kembali ke Atas</a>

</div>
