# Gio AI

**Assistente pessoal com IA para pessoas 45+**, contratado por familiares que querem oferecer suporte e companhia com tecnologia de ponta — sem complicação para quem usa.

---

## O que é o Gio

O Gio é um assistente que conversa, lembra, orienta e acompanha. Quem usa não precisa saber que está usando IA — só precisa falar com o Gio.

Quem contrata (filhos, netos, cônjuges) configura o tom, os tópicos preferidos e o nível de suporte através de um console dedicado.

---

## Repositórios

| Repo | Descrição |
|------|-----------|
| [gio-backend](https://github.com/gio-concierge/gio-backend) | API em Go + Fiber — autenticação OTP/JWT, conversa com IA, roteamento de providers |
| [gio-app](https://github.com/gio-concierge/gio-app) | App Flutter — interface do usuário 45+ e console do assinante (iOS, Android, Web) |
| [gio-docs](https://github.com/gio-concierge/gio-docs) | Documentação técnica e docs-for-dummies com analogias |
| [gio-ai](https://github.com/gio-concierge/gio-ai) | Pipeline de fine-tune, scripts de treinamento e avaliação do modelo |
| [gio-infra](https://github.com/gio-concierge/gio-infra) | Infraestrutura — Docker, Terraform, CI/CD e configs de deploy |

---

## Stack

**Backend** — Go · Fiber · JWT · Resend · Groq (Llama 3.3 70B) · Claude Haiku  
**App** — Flutter · GoRouter · SharedPreferences  
**Infra** — VPS AlmaLinux · Docker · OpenLiteSpeed · Let's Encrypt · GitHub Actions  
**Banco (em breve)** — PostgreSQL · pgvector

---

## Produto em produção

| | |
|-|-|
| App | [app.gioai.com.br](https://app.gioai.com.br) |
| Site | [gioai.com.br](https://gioai.com.br) |
