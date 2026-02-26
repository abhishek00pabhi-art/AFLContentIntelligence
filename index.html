import { useState, useRef } from "react";

const BRAND_CONTEXT = `You are a research and content agent for Asha's Fresh Look, a luxury beauty salon and academy brand based in Sikar, Rajasthan, India.

KEY BRAND FACTS:
- Founded by Asha Choudhary, CEO & Founder — a certified cosmetologist, makeup artist, and distinguished entrepreneur
- 25+ years of excellence in the beauty industry
- 1.5 Lakh (150,000+) happy clients served over 25 years
- 3 branches in Sikar: Tabela Market (+91 8696228888), Bioscope Mall (+91 8696238888), Salasar Stand (+91 8696218888)
- 50+ beauticians, 25+ hairdressers on team
- Winner of 25+ industry awards
- Rated EXCELLENT — 1428+ Google reviews
- Known as the Best Bridal Makeup Studio & Best Salon in Sikar / Shekhawati region / Rajasthan

AFL ACADEMY (AFL Hair & Beauty Academy):
- International Certified Faculty: City & Guilds (UK), Toni & Guy, L'Oréal Professional certified instructors
- ONLY IHB Approved Institute in Sikar and nearby territories
- Live salon setup — real clients from Month 2 onwards
- 100% Placement Assistance — graduates placed at Lakmé Salon, BBlunt, salons in Jaipur, Delhi, Mumbai
- 2,000+ alumni
- Residential facility for female students available
- Includes business training: how to start your own salon (costs, marketing, client management)
- Professional portfolio photoshoot included in course fee
- Toolkits and products available at wholesale prices

SERVICES OFFERED: Hair (cuts, color, keratin, smoothening, extensions), Skin (facials, anti-ageing, glow, tan removal, acne), Nail Extensions, Bridal Makeup (airbrush, reception, engagement, full bridal), SPA, Hand & Feet, Advanced Treatments. Also destination bridal makeup across Rajasthan.

FRANCHISE: Multi-award-winning brand offering franchise partners complete business guidance — from setup to growth.

ASHA CHOUDHARY — CEO VOICE & PERSONA:
- Empowering, warm, and deeply passionate about beauty as self-expression
- Believes true beauty glows from within
- Champion of women's empowerment through beauty education in Tier-2 cities
- Pioneering luxury beauty standards in non-metro Rajasthan
- Personal, authentic, community-first, visionary
- Often speaks about giving women confidence and career opportunities

Website: ashafreshlook.com | Email: info@ashafreshlook.com | Instagram: @ashafreshlook`;

const QUICK_PROMPTS = [
  { icon: "🌟", label: "CEO Bio for Instagram", prompt: "Write a compelling Instagram bio for Asha Choudhary, CEO & Founder of Asha's Fresh Look. Make it punchy, inspiring, and include key highlights of her 25-year journey." },
  { icon: "✍️", label: "Brand Story (3 Paragraphs)", prompt: "Write the brand story of Asha's Fresh Look in 3 paragraphs — the origin, the growth, and the vision for the future. It should feel like it comes directly from Asha Choudhary herself." },
  { icon: "📣", label: "5 Instagram Captions", prompt: "Give 5 Instagram caption ideas for Asha's Fresh Look. Mix bridal, academy, salon lifestyle, and motivational themes. Include relevant hashtags for each." },
  { icon: "🎓", label: "Academy Announcement", prompt: "Write a social media announcement post for AFL Hair & Beauty Academy highlighting its City & Guilds certification, IHB approval, 100% placement record, and Asha's vision to empower women through beauty education." },
  { icon: "👰", label: "Bridal Season Promo", prompt: "Write promotional copy for Asha's Fresh Look's bridal packages for the 2026 wedding season. Highlight airbrush makeup, reception and engagement looks, and the team's 25 years of expertise." },
  { icon: "🏢", label: "Franchise Pitch", prompt: "Write a compelling franchise pitch from Asha Choudhary to prospective partners — covering the brand's 25-year track record, support system, awards, and opportunity in Rajasthan's growing beauty market." },
  { icon: "💬", label: "CEO Quotes on Beauty", prompt: "Write 3 powerful, quotable statements from Asha Choudhary about beauty, empowerment, and entrepreneurship in the Indian beauty industry. These should be authentic and shareable on LinkedIn or Instagram." },
  { icon: "📰", label: "Press Release – New Branch", prompt: "Write a press release announcing a new Asha's Fresh Look branch opening in a new Rajasthan city. Include brand stats and a quote from CEO Asha Choudhary." },
];

const TONES = ["Professional", "Inspirational", "Warm & Personal", "Luxurious & Refined", "Bold & Empowering"];

export default function App() {
  const [prompt, setPrompt] = useState("");
  const [tone, setTone] = useState("Professional");
  const [output, setOutput] = useState("");
  const [loading, setLoading] = useState(false);
  const [history, setHistory] = useState([]);
  const [copied, setCopied] = useState(false);
  const outputRef = useRef(null);

  async function runResearch() {
    if (!prompt.trim() || loading) return;
    setLoading(true);
    setOutput("");

    const systemPrompt = `${BRAND_CONTEXT}\n\nYou are writing content for Asha Choudhary or Asha's Fresh Look brand. Tone: ${tone}.\n\nRules:\n- Keep content on-brand: warm, professional, empowering\n- Reference specific brand facts where relevant\n- Write in clean, copy-ready format\n- If writing in Asha's voice, make it personal and authentic\n- No generic filler; every line should earn its place`;

    try {
      const res = await fetch("https://api.anthropic.com/v1/messages", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          model: "claude-sonnet-4-20250514",
          max_tokens: 1000,
          system: systemPrompt,
          messages: [{ role: "user", content: prompt }]
        })
      });
      const data = await res.json();
      const text = data.content?.map(b => b.text || "").join("") || "No response.";
      setOutput(text);
      setHistory(h => [{ q: prompt, a: text, time: new Date().toLocaleTimeString() }, ...h].slice(0, 6));
      setTimeout(() => outputRef.current?.scrollIntoView({ behavior: "smooth" }), 100);
    } catch (e) {
      setOutput("Error: " + e.message);
    }
    setLoading(false);
  }

  function copyOutput() {
    navigator.clipboard.writeText(output).then(() => {
      setCopied(true);
      setTimeout(() => setCopied(false), 2000);
    });
  }

  const gold = "#C9A96E";
  const deep = "#1A0F0A";
  const warm = "#2D1B12";
  const cream = "#F5EFE6";
  const muted = "#8A7060";
  const border = "rgba(201,169,110,0.22)";

  return (
    <div style={{ background: deep, minHeight: "100vh", fontFamily: "'Georgia', serif", color: cream, padding: "0 0 80px" }}>
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap');
        * { box-sizing: border-box; }
        textarea { font-family: 'DM Sans', sans-serif !important; }
        textarea::placeholder { color: ${muted}; }
        ::-webkit-scrollbar { width: 4px; } 
        ::-webkit-scrollbar-track { background: transparent; }
        ::-webkit-scrollbar-thumb { background: rgba(201,169,110,0.3); border-radius: 4px; }
        .quick-btn:hover { background: rgba(201,169,110,0.1) !important; border-color: rgba(201,169,110,0.5) !important; }
        .run-btn:hover { opacity: 0.88 !important; }
        .run-btn:disabled { opacity: 0.45 !important; cursor: not-allowed !important; }
        .hist-item:hover { border-left-color: ${gold} !important; background: rgba(201,169,110,0.05) !important; }
      `}</style>

      <div style={{ maxWidth: 760, margin: "0 auto", padding: "40px 20px 0" }}>

        {/* Header */}
        <div style={{ textAlign: "center", marginBottom: 36 }}>
          <div style={{ display: "inline-flex", alignItems: "center", gap: 8, background: "rgba(201,169,110,0.1)", border: `1px solid ${border}`, borderRadius: 100, padding: "5px 18px", fontSize: 11, letterSpacing: "0.14em", textTransform: "uppercase", color: gold, marginBottom: 18, fontFamily: "'DM Sans', sans-serif" }}>
            ✦ Asha's Fresh Look · Research Agent
          </div>
          <h1 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(26px,5vw,40px)", fontWeight: 700, lineHeight: 1.2, margin: "0 0 8px" }}>
            Content Intelligence for<br />
            <em style={{ color: gold, fontStyle: "italic" }}>Asha Choudhary</em>
          </h1>
          <p style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 14, color: muted, maxWidth: 420, margin: "10px auto 0", lineHeight: 1.6 }}>
            AI research assistant pre-loaded with full brand context. Ask anything about AFL's story, CEO voice, or content ideas.
          </p>
          <div style={{ display: "flex", flexWrap: "wrap", gap: 7, justifyContent: "center", marginTop: 16 }}>
            {["🏆 CEO & Founder", "📍 Sikar, Rajasthan", "✨ 25 Years", "🎓 AFL Academy", "👰 Bridal Expert"].map(c => (
              <span key={c} style={{ background: "rgba(255,255,255,0.04)", border: `1px solid ${border}`, borderRadius: 100, padding: "3px 12px", fontSize: 11, color: muted, fontFamily: "'DM Sans', sans-serif" }}>{c}</span>
            ))}
          </div>
        </div>

        {/* Stats */}
        <div style={{ display: "grid", gridTemplateColumns: "repeat(5,1fr)", gap: 1, background: border, border: `1px solid ${border}`, borderRadius: 12, overflow: "hidden", marginBottom: 28 }}>
          {[["1.5L+","Happy Clients"],["25+","Awards"],["3","Branches"],["50+","Beauticians"],["2K+","Alumni"]].map(([n,l]) => (
            <div key={l} style={{ background: "rgba(255,255,255,0.02)", padding: "14px 12px", textAlign: "center" }}>
              <div style={{ fontFamily: "'Playfair Display', serif", fontSize: 20, color: gold, fontWeight: 700 }}>{n}</div>
              <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, color: muted, marginTop: 3 }}>{l}</div>
            </div>
          ))}
        </div>

        {/* Quick Prompts */}
        <div style={{ marginBottom: 24 }}>
          <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, letterSpacing: "0.12em", textTransform: "uppercase", color: muted, marginBottom: 12 }}>✦ Quick Prompts</div>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill,minmax(170px,1fr))", gap: 8 }}>
            {QUICK_PROMPTS.map(({ icon, label, prompt: p }) => (
              <button key={label} className="quick-btn" onClick={() => setPrompt(p)}
                style={{ background: "rgba(255,255,255,0.025)", border: `1px solid ${border}`, borderRadius: 10, color: cream, fontFamily: "'DM Sans', sans-serif", fontSize: 13, padding: "11px 13px", cursor: "pointer", textAlign: "left", lineHeight: 1.4, transition: "all 0.2s" }}>
                <div style={{ fontSize: 16, marginBottom: 4 }}>{icon}</div>
                {label}
              </button>
            ))}
          </div>
        </div>

        {/* Input */}
        <div style={{ background: "rgba(255,255,255,0.03)", border: `1px solid ${border}`, borderRadius: 14, padding: "18px 20px", marginBottom: 24 }}>
          <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, letterSpacing: "0.12em", textTransform: "uppercase", color: gold, marginBottom: 12 }}>✦ Your Research Request</div>
          <textarea
            value={prompt}
            onChange={e => setPrompt(e.target.value)}
            onKeyDown={e => e.ctrlKey && e.key === "Enter" && runResearch()}
            rows={4}
            placeholder="e.g. Write a LinkedIn post from Asha Choudhary about empowering women through beauty education in Rajasthan…"
            style={{ width: "100%", background: "transparent", border: "none", outline: "none", color: cream, fontSize: 15, lineHeight: 1.65, resize: "none" }}
          />
          <div style={{ display: "flex", alignItems: "center", justifyContent: "space-between", marginTop: 14, gap: 10 }}>
            <select value={tone} onChange={e => setTone(e.target.value)}
              style={{ background: "rgba(255,255,255,0.05)", border: `1px solid ${border}`, borderRadius: 8, color: cream, fontFamily: "'DM Sans', sans-serif", fontSize: 13, padding: "8px 12px", cursor: "pointer", outline: "none", flex: 1, maxWidth: 220 }}>
              {TONES.map(t => <option key={t} value={t} style={{ background: warm }}>Tone: {t}</option>)}
            </select>
            <button className="run-btn" onClick={runResearch} disabled={loading || !prompt.trim()}
              style={{ background: `linear-gradient(135deg, ${gold}, #9A7030)`, border: "none", borderRadius: 10, color: deep, fontFamily: "'DM Sans', sans-serif", fontWeight: 600, fontSize: 14, padding: "10px 26px", cursor: "pointer", transition: "opacity 0.2s", whiteSpace: "nowrap" }}>
              {loading ? "Researching…" : "Research ✦"}
            </button>
          </div>
        </div>

        {/* Output */}
        {(loading || output) && (
          <div ref={outputRef}>
            <div style={{ background: "rgba(255,255,255,0.025)", border: `1px solid ${border}`, borderRadius: 14, overflow: "hidden" }}>
              <div style={{ display: "flex", alignItems: "center", justifyContent: "space-between", padding: "12px 20px", borderBottom: `1px solid ${border}`, background: "rgba(201,169,110,0.06)" }}>
                <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, letterSpacing: "0.12em", textTransform: "uppercase", color: gold }}>✦ Research Output</div>
                {output && (
                  <button onClick={copyOutput}
                    style={{ background: "transparent", border: `1px solid ${border}`, borderRadius: 6, color: copied ? gold : muted, fontFamily: "'DM Sans', sans-serif", fontSize: 12, padding: "4px 12px", cursor: "pointer", transition: "all 0.2s" }}>
                    {copied ? "Copied ✓" : "Copy"}
                  </button>
                )}
              </div>
              <div style={{ padding: "22px 24px", fontFamily: "'DM Sans', sans-serif", fontSize: 14.5, lineHeight: 1.8, color: cream, minHeight: 80, whiteSpace: "pre-wrap" }}>
                {loading ? (
                  <div style={{ display: "flex", gap: 6, alignItems: "center", padding: "8px 0" }}>
                    {[0, 0.2, 0.4].map((d, i) => (
                      <div key={i} style={{ width: 8, height: 8, borderRadius: "50%", background: gold, animation: `bounce 1.2s ${d}s ease-in-out infinite`, opacity: 0.7 }} />
                    ))}
                    <style>{`@keyframes bounce { 0%,80%,100%{transform:scale(0.6);opacity:0.4} 40%{transform:scale(1);opacity:1} }`}</style>
                  </div>
                ) : output}
              </div>
            </div>
          </div>
        )}

        {/* History */}
        {history.length > 1 && (
          <div style={{ marginTop: 32 }}>
            <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, letterSpacing: "0.12em", textTransform: "uppercase", color: muted, marginBottom: 12 }}>✦ Session History</div>
            {history.slice(1).map((item, i) => (
              <div key={i} className="hist-item" onClick={() => { setPrompt(item.q); setOutput(item.a); }}
                style={{ padding: "10px 16px", borderLeft: `2px solid ${border}`, marginBottom: 8, cursor: "pointer", transition: "all 0.2s", borderRadius: "0 6px 6px 0" }}>
                <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 13, color: muted, whiteSpace: "nowrap", overflow: "hidden", textOverflow: "ellipsis" }}>{item.q}</div>
                <div style={{ fontFamily: "'DM Sans', sans-serif", fontSize: 11, color: "rgba(138,112,96,0.55)", marginTop: 2 }}>{item.time}</div>
              </div>
            ))}
          </div>
        )}

      </div>
    </div>
  );
}
