ZENVORO MVP setup
1) Install Node.js LTS: https://nodejs.org
2) Copy .env.example to .env; fill Supabase Project URL + Publishable key (Settings > API Keys).
3) Open Command Prompt in this folder: npm install then npm run dev
4) Open localhost URL shown.
Admin after signup: update public.profiles set role='admin' where email='YOUR_EMAIL';
VIP manual: update public.profiles set vip_active=true,vip_until=now()+interval '30 days' where email='MEMBER_EMAIL';
Never use secret/service_role key in browser. Prototype only; add server-side payment verification before charging customers.