import React, { useEffect, useMemo, useState } from "react";

// =====================================================================
// NTO BRASIL — Site oficial COMPLETO (tema claro fixo + refinado)
// Seções: Hero (logo grande), Mensagem (texto completo), Mapa, Posts,
// Conhecimento, Galeria, Sobre, FAQ, Contato. CTA flutuante incluso.
// Animações suaves via IntersectionObserver (Reveal) + CSS injetado.
// =====================================================================

const SITE_NAME = "NTO – Brasil";
const LOGO_URL = "/mnt/data/LOGO OFICIAL NTO  (1).png"; // logo enviada
const CONTACT_EMAIL = "admn@ntobr.com";

const SOCIAL = {
  instagramEmbedUrl: "https://www.instagram.com/p/Ck000000000/embed", // troque pelo embed oficial do perfil
  youtubeEmbedUrl: "https://www.youtube.com/embed/dQw4w9WgXcQ", // troque pelo vídeo/playlists oficiais
};

// ===== Utilidades =====
function useSEO() {
  useEffect(() => {
    document.title = `${SITE_NAME} — Psicodélicos com ciência, ética e cuidado`;
    // favicon
    let link = document.querySelector("link[rel='icon']");
    if (!link) {
      link = document.createElement("link");
      link.rel = "icon";
      document.head.appendChild(link);
    }
    link.href = LOGO_URL;

    // rolagem suave
    try {
      document.documentElement.style.scrollBehavior = "smooth";
    } catch {}

    // CSS de animação (fade + slide)
    const styleId = "nto-anim-base";
    if (!document.getElementById(styleId)) {
      const s = document.createElement("style");
      s.id = styleId;
      s.innerHTML = `
        .reveal{opacity:0;transform:translateY(14px);transition:opacity .6s ease,transform .6s ease}
        .reveal.is-visible{opacity:1;transform:none}
      `;
      document.head.appendChild(s);
    }
  }, []);
}

// IntersectionObserver para revelar elementos ao rolar
function Reveal({ children, className, style }) {
  const ref = React.useRef(null);
  useEffect(() => {
    const el = ref.current;
    if (!el) return;
    const io = new IntersectionObserver(
      (entries) => {
        entries.forEach((e) => {
          if (e.isIntersecting) {
            e.target.classList.add("is-visible");
            io.unobserve(e.target);
          }
        });
      },
      { rootMargin: "0px 0px -10% 0px", threshold: 0.15 }
    );
    io.observe(el);
    return () => io.disconnect();
  }, []);
  return (
    <div ref={ref} className={`reveal ${className || ""}`} style={style}>
      {children}
    </div>
  );
}

function Section({ id, title, subtitle, children, pad = true }) {
  return (
    <section id={id} className={`relative ${pad ? "py-20" : "py-0"}`}>
      <div className="relative mx-auto max-w-6xl px-6">
        <Reveal>
          {title && (
            <div className="mb-8 text-center">
              <h2 className="text-3xl md:text-4xl font-serif font-semibold text-slate-900">
                {title}
              </h2>
              {subtitle && (
                <p className="mt-2 text-slate-600 text-lg">{subtitle}</p>
              )}
            </div>
          )}
          {children}
        </Reveal>
      </div>
    </section>
  );
}

function CTAButton({ href, children }) {
  return (
    <a
      href={href}
      className="inline-flex items-center rounded-full px-8 py-3 text-lg font-medium bg-gradient-to-r from-emerald-500 via-cyan-500 to-violet-600 text-white shadow-lg hover:opacity-90 transition-transform duration-300 hover:scale-105"
    >
      {children}
    </a>
  );
}

// ===== Seções =====
function Hero() {
  return (
    <section id="hero" className="relative overflow-hidden">
      {/* mesh gradient de fundo */}
      <div className="absolute inset-0 -z-10 bg-[radial-gradient(1200px_600px_at_10%_-20%,#dcfce7_0%,transparent_60%),radial-gradient(900px_500px_at_110%_30%,#e9d5ff_0%,transparent_55%),radial-gradient(600px_400px_at_50%_120%,#bae6fd_0%,transparent_60%)]" />
      <Reveal className="mx-auto max-w-6xl px-6 pt-20 pb-20 flex flex-col items-center text-center">
        <img
          src={LOGO_URL}
          alt="NTO Brasil"
          className="h-48 md:h-64 w-auto mb-8 drop-shadow-xl"
        />
        <h1 className="text-4xl md:text-5xl font-serif font-bold tracking-tight text-slate-900">
          Ciência, ética e cuidado
        </h1>
        <p className="mt-4 max-w-2xl text-lg text-slate-700">
          Alívio com dignidade para quem carrega um peso insuportável. A NTO
          caminha com você.
        </p>
        <div className="mt-8 flex gap-4 flex-wrap justify-center">
          <CTAButton
            href={`mailto:${CONTACT_EMAIL}?subject=${encodeURIComponent(
              "Quero aliviar meu sofrimento"
            )}`}
          >
            QUERO ALÍVIO 🫶
          </CTAButton>
          <a
            href="#conhecimento"
            className="inline-flex items-center rounded-full px-8 py-3 text-lg font-medium border border-slate-300 bg-white shadow-sm hover:bg-slate-50"
          >
            Conhecimento
          </a>
        </div>
      </Reveal>
    </section>
  );
}

function SocialEmbeds() {
  return (
    <div className="grid gap-8 md:grid-cols-2">
      <iframe
        title="Instagram"
        src={SOCIAL.instagramEmbedUrl}
        loading="lazy"
        className="w-full h-[500px] rounded-xl border"
      />
      <iframe
        title="YouTube"
        src={SOCIAL.youtubeEmbedUrl}
        loading="lazy"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowFullScreen
        className="w-full h-[500px] rounded-xl border"
      />
    </div>
  );
}

function KnowledgeCards() {
  const KNOWLEDGE = [
    { id: "cetamina", title: "Cetamina", text: "Alívio rápido em depressão resistente. Infusão/spray supervisionado." },
    { id: "ibogaina", title: "Ibogaína", text: "Protocolos em dependência. Monitorização multiprofissional." },
    { id: "psilocibina", title: "Psilocibina", text: "Pesquisada em depressão/ansiedade. Sessões assistidas com integração." },
    { id: "lsd", title: "LSD", text: "Investigada em contextos de pesquisa. Set & setting estruturados." },
    { id: "ayahuasca", title: "Ayahuasca", text: "Uso religioso protegido no Brasil. Contextos ritualísticos." },
    { id: "mdma", title: "MDMA", text: "Estudos em TEPT. Psicoterapia assistida." },
  ];
  const [q, setQ] = useState("");
  const data = useMemo(
    () => KNOWLEDGE.filter((k) => !q || k.title.toLowerCase().includes(q.toLowerCase())),
    [q]
  );
  return (
    <div>
      <input
        value={q}
        onChange={(e) => setQ(e.target.value)}
        placeholder="Buscar psicodélico"
        className="mb-6 w-full md:w-1/2 rounded-full border border-slate-300 px-5 py-2 text-base shadow-sm"
      />
      <div className="grid gap-8 md:grid-cols-2 lg:grid-cols-3">
        {data.map((k, i) => (
          <Reveal key={k.id} style={{ transitionDelay: `${i * 80}ms` }}>
            <article className="rounded-3xl border border-slate-200 bg-white p-6 shadow-md hover:shadow-lg transition">
              <h3 className="text-xl font-semibold text-slate-900">{k.title}</h3>
              <p className="mt-2 text-slate-600">{k.text}</p>
            </article>
          </Reveal>
        ))}
      </div>
    </div>
  );
}

function Gallery() {
  const IMGS = [
    { src: "https://images.unsplash.com/photo-1520975922284-9f786f2de3aa?q=80&w=1400&auto=format&fit=crop", alt: "Floresta amazônica" },
    { src: "https://images.unsplash.com/photo-1549880338-65ddcdfd017b?q=80&w=1400&auto=format&fit=crop", alt: "Céu estrelado" },
    { src: "https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?q=80&w=1400&auto=format&fit=crop", alt: "Montanhas" },
  ];
  return (
    <div className="grid gap-6 md:grid-cols-3">
      {IMGS.map((i, idx) => (
        <Reveal key={i.src} style={{ transitionDelay: `${idx * 90}ms` }}>
          <figure className="overflow-hidden rounded-3xl border border-slate-200 bg-white shadow-md">
            <img
              src={i.src}
              alt={i.alt}
              className="h-64 w-full object-cover transition-transform duration-500 hover:scale-105"
            />
            <figcaption className="p-3 text-center text-sm text-slate-600">
              {i.alt}
            </figcaption>
          </figure>
        </Reveal>
      ))}
    </div>
  );
}

function FAQ() {
  const items = [
    { q: "A NTO atende urgências?", a: "Fazemos avaliação rápida para avaliar risco e opções clínicas." },
    { q: "Cetamina é para todo mundo?", a: "Não. Exige triagem médica e pode ter contraindicações." },
    { q: "Como funcionam as sessões?", a: "Preparação, sessão monitorada e integração pós-sessão." },
  ];
  const [open, setOpen] = useState(0);
  return (
    <div className="mx-auto max-w-3xl">
      {items.map((it, i) => (
        <Reveal key={it.q} style={{ transitionDelay: `${i * 100}ms` }}>
          <div className="border-b border-slate-200">
            <button
              onClick={() => setOpen(open === i ? null : i)}
              className="w-full py-4 flex items-center justify-between text-left"
            >
              <span className="text-lg font-medium text-slate-900">{it.q}</span>
              <span className="text-slate-500">{open === i ? "−" : "+"}</span>
            </button>
            {open === i && <p className="pb-4 text-slate-600">{it.a}</p>}
          </div>
        </Reveal>
      ))}
    </div>
  );
}

function FloatingCTA() {
  return (
    <a
      href={`mailto:${CONTACT_EMAIL}?subject=${encodeURIComponent(
        "Quero aliviar meu sofrimento"
      )}`}
      className="fixed bottom-6 right-6 z-50 inline-flex items-center rounded-full px-6 py-3 text-base font-medium bg-gradient-to-r from-emerald-500 via-cyan-500 to-violet-600 text-white shadow-xl hover:opacity-90 transition-transform duration-300 hover:scale-105"
    >
      🫶 Quero Alívio
    </a>
  );
}

// ===== App =====
export default function NTOBrasilSite() {
  useSEO();
  const [mobileOpen, setMobileOpen] = useState(false);

  // Smoke tests (não quebram o app): garantem que IDs essenciais existem
  useEffect(() => {
    const ids = [
      "mensagem",
      "mapa",
      "posts",
      "conhecimento",
      "galeria",
      "sobre",
      "faq",
      "contato",
    ];
    const missing = ids.filter((id) => !document.getElementById(id));
    if (missing.length) console.warn("[NTO] Seções ausentes:", missing.join(", "));
  }, []);

  return (
    <div className="min-h-screen bg-gradient-to-br from-slate-50 via-white to-slate-100 text-slate-800">
      {/* Header */}
      <header className="sticky top-0 z-50 bg-white/90 backdrop-blur border-b border-slate-200 shadow-sm">
        <div className="mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
          <a href="#home" className="flex items-center gap-3">
            <img
              src={LOGO_URL}
              alt="Logo NTO"
              width={70}
              height={70}
              className="object-contain"
            />
            <span className="text-2xl font-serif font-semibold tracking-wide text-slate-900">
              BRASIL
            </span>
          </a>
          <nav className="hidden md:flex items-center gap-6 text-sm font-medium">
            {[
              "Home",
              "Mensagem",
              "Mapa",
              "Posts",
              "Conhecimento",
              "Galeria",
              "Sobre",
              "FAQ",
              "Contato",
            ].map((label) => (
              <a
                key={label}
                href={`#${label.toLowerCase()}`}
                className="text-slate-700 hover:text-emerald-600 transition-colors duration-300"
              >
                {label}
              </a>
            ))}
            <CTAButton
              href={`mailto:${CONTACT_EMAIL}?subject=${encodeURIComponent(
                "Quero aliviar meu sofrimento"
              )}`}
            >
              QUERO ALÍVIO 🫶
            </CTAButton>
          </nav>
          <button
            className="md:hidden px-3 py-2 border border-slate-300 rounded-lg"
            onClick={() => setMobileOpen((v) => !v)}
          >
            ☰
          </button>
        </div>
        {mobileOpen && (
          <div className="md:hidden border-t border-slate-200 bg-white/95 px-6 py-4 flex flex-col gap-3">
            {[
              "Home",
              "Mensagem",
              "Mapa",
              "Posts",
              "Conhecimento",
              "Galeria",
              "Sobre",
              "FAQ",
              "Contato",
            ].map((label) => (
              <a
                key={label}
                href={`#${label.toLowerCase()}`}
                className="text-slate-700 hover:text-emerald-600"
              >
                {label}
              </a>
            ))}
            <CTAButton
              href={`mailto:${CONTACT_EMAIL}?subject=${encodeURIComponent(
                "Quero aliviar meu sofrimento"
              )}`}
            >
              QUERO ALÍVIO 🫶
            </CTAButton>
          </div>
        )}
      </header>

      {/* Conteúdo principal */}
      <main id="home">
        <Hero />

        {/* MENSAGEM — texto completo, sem perder nada */}
        <Section
          id="mensagem"
          title="Mensagem da NTO – Brasil"
          subtitle="Carinho, ciência e responsabilidade"
        >
          <div className="rounded-3xl border border-slate-200 bg-white p-8 shadow-md text-slate-700 space-y-4">
            <p>
              A NTO acredita que psicodélicos, quando usados com ciência, ética e
              carinho, podem abrir uma janela real de alívio — especialmente para
              quem já tentou “de tudo” e continua carregando um peso insuportável.
              <strong> Não é fuga. É cuidado.</strong>
            </p>
            <p>
              Psicodélicos são ferramentas terapêuticas que, em ambiente clínico
              supervisionado, favorecem neuroplasticidade e flexibilizam padrões
              rígidos de pensamento ligados à depressão, à urgência suicida e a
              certos quadros de dependência. No Brasil, a cetamina (e o spray de
              esketamina) já está disponível legalmente em contexto médico e pode
              oferecer alívio em horas ou poucos dias, enquanto o tratamento de
              base continua a agir.
            </p>
            <h3 className="text-xl font-semibold text-slate-900">
              Por que considerar agora
            </h3>
            <p>
              Quando a dor aperta, esperar semanas por resposta é cruel. A cetamina
              pode funcionar como “bote salva-vidas”: reduz a intensidade do
              sofrimento, baixa o volume da ideação suicida e devolve fôlego para
              retomar o plano terapêutico com mais clareza.
            </p>
            <h3 className="text-xl font-semibold text-slate-900">
              Como cuidamos de você na NTO – Brasil
            </h3>
            <ul className="list-disc pl-5 space-y-1">
              <li>
                <strong>Avaliação médica rigorosa:</strong> entendemos sua
                história, riscos e objetivos.
              </li>
              <li>
                <strong>Sessões seguras (infusão/spray):</strong> monitorização
                contínua, conforto e presença.
              </li>
              <li>
                <strong>Integração pós-sessão:</strong> transformamos a
                experiência em mudanças concretas de vida.
              </li>
              <li>
                <strong>Plano personalizado:</strong> combinamos com psicoterapia
                e ajustes de medicação, quando indicado.
              </li>
            </ul>
            <h3 className="text-xl font-semibold text-slate-900">
              O que você pode esperar
            </h3>
            <p>
              Durante a sessão, podem ocorrer sensações dissociativas
              (distanciamento, alteração de percepção) que passam rápido. Alguns
              sentem alívio emocional, outros descrevem um “respiro” onde antes só
              havia peso. Resultados variam — nossa promessa é cuidado sério,
              transparente e humano.
            </p>
            <h3 className="text-xl font-semibold text-slate-900">
              Para quem pode ajudar
            </h3>
            <ul className="list-disc pl-5 space-y-1">
              <li>Depressão resistente a tratamentos anteriores.</li>
              <li>Ideação suicida ou agravamento agudo do sofrimento.</li>
              <li>
                Ansiedade grave, TEPT e uso problemático de substâncias (em
                protocolos específicos e baseados em evidências emergentes).
              </li>
            </ul>
            <h3 className="text-xl font-semibold text-slate-900">
              Transparência é respeito
            </h3>
            <p>
              A cetamina não é para todos. Contraindicações e cautelas incluem:
              hipertensão não controlada, cardiopatia instável, gravidez, psicose
              ativa, fase maníaca e histórico de uso indevido de dissociativos. Por
              isso sempre fazemos triagem e acompanhamos de perto.
            </p>
            <blockquote className="border-l-4 border-slate-300 pl-4 text-slate-800">
              Você não é seu diagnóstico. Você é alguém que sofre — e merece
              alívio, com dignidade e ciência do seu lado. A gente caminha com
              você, passo a passo, até a vida voltar a caber no peito.
            </blockquote>
            <div className="pt-2">
              <CTAButton
                href={`mailto:${CONTACT_EMAIL}?subject=${encodeURIComponent(
                  "Quero aliviar meu sofrimento"
                )}`}
              >
                QUERO ALÍVIO 🫶
              </CTAButton>
            </div>
          </div>
        </Section>

        {/* MAPA */}
        <Section
          id="mapa"
          title="Mapa Psicodélico"
          subtitle="Pontos públicos em Google My Maps"
        >
          <div className="rounded-3xl border border-slate-200 bg-white p-4 shadow-md">
            <iframe
              src="https://www.google.com/maps/d/embed?mid=1KD5QHhxyVWlFX7BDM0aoNufixLILENU&usp=sharing"
              className="w-full h-[480px] rounded-xl"
              loading="lazy"
            />
          </div>
        </Section>

        {/* POSTS */}
        <Section
          id="posts"
          title="Redes da NTO"
          subtitle="Atualizações do Instagram e YouTube"
        >
          <SocialEmbeds />
        </Section>

        {/* CONHECIMENTO */}
        <Section
          id="conhecimento"
          title="Conhecimento"
          subtitle="Resumo responsável + links de referência"
        >
          <KnowledgeCards />
        </Section>

        {/* GALERIA */}
        <Section
          id="galeria"
          title="Imagens"
          subtitle="Espaço para fotos de alto impacto visual"
        >
          <Gallery />
        </Section>

        {/* SOBRE */}
        <Section id="sobre" title="Sobre">
          <div className="rounded-3xl border border-slate-200 bg-white p-8 shadow-md text-slate-700 space-y-3">
            <p>
              <strong>Somos Produtora, Editora, Tradutora.</strong> Instituto
              médico e multidisciplinar de pesquisa, estudo e promoção de
              enteógenos para fins de proteção à vida.
            </p>
            <ul className="list-disc pl-5">
              <li>
                <strong>Valores</strong>: Ciência, Espiritualidade, Sabedoria,
                Transcendência.
              </li>
              <li>
                <strong>Missão</strong>: Aliviar o sofrimento humano através dos
                enteógenos.
              </li>
              <li>
                <strong>Visão</strong>: Ser peça fundamental para a revolução
                psicodélica do século XXI no Brasil.
              </li>
            </ul>
          </div>
        </Section>

        {/* FAQ */}
        <Section
          id="faq"
          title="Perguntas Frequentes"
          subtitle="As dúvidas mais comuns, respondidas de forma direta"
        >
          <FAQ />
        </Section>

        {/* CONTATO */}
        <Section id="contato" title="Contato">
          <div className="rounded-3xl border border-slate-200 bg-white p-8 shadow-md text-slate-700">
            <p className="text-lg">
              Email:{" "}
              <a className="underline" href={`mailto:${CONTACT_EMAIL}`}>
                {CONTACT_EMAIL}
              </a>
            </p>
            <p className="mt-2 text-sm text-slate-600">
              Preferimos comunicação assíncrona, curta e objetiva. Para assuntos
              clínicos, evite dados sensíveis sem canal seguro.
            </p>
          </div>
        </Section>
      </main>

      {/* CTA flutuante */}
      <FloatingCTA />
    </div>
  );
}

