import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { motion } from "framer-motion";
import { Star } from "lucide-react";

export default function LandingPage() {
  return (
    <div className="bg-gradient-to-b from-[#0f0c29] via-[#302b63] to-[#24243e] text-white min-h-screen font-sans">
      {/* Hero Section */}
      <section className="text-center py-24 px-6 max-w-4xl mx-auto">
        <motion.h1 
          className="text-5xl md:text-6xl font-bold mb-6"
          initial={{ opacity: 0, y: -20 }} 
          animate={{ opacity: 1, y: 0 }} 
          transition={{ duration: 0.8 }}
        >
          Transforme sua produtividade com nossa solução SaaS
        </motion.h1>
        <p className="text-lg md:text-xl mb-8 text-zinc-300">
          Interface intuitiva, poderosa e feita para equipes modernas.
        </p>
        <Button className="text-lg px-6 py-4 rounded-2xl shadow-xl bg-gradient-to-r from-blue-500 to-violet-600 hover:opacity-90">
          Experimente Grátis
        </Button>
      </section>

      {/* Tabela de Preços */}
      <section className="py-20 px-4 bg-zinc-900">
        <h2 className="text-4xl font-bold text-center mb-12">Planos & Preços</h2>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
          {["Starter", "Pro", "Enterprise"].map((tier, i) => (
            <Card key={tier} className="bg-zinc-800 text-white border border-zinc-700">
              <CardContent className="p-6 text-center">
                <h3 className="text-2xl font-semibold mb-4">{tier}</h3>
                <p className="text-4xl font-bold mb-4">
                  {i === 0 ? "R$ 0" : i === 1 ? "R$ 49" : "R$ 199"}
                  <span className="text-sm font-normal text-zinc-400">/mês</span>
                </p>
                <ul className="text-zinc-300 mb-6 space-y-2">
                  <li>Recursos ilimitados</li>
                  <li>Colaboração em tempo real</li>
                  <li>Suporte {i === 2 ? "prioritário" : "padrão"}</li>
                </ul>
                <Button className="w-full bg-gradient-to-r from-blue-500 to-violet-600 hover:opacity-90">
                  Começar agora
                </Button>
              </CardContent>
            </Card>
          ))}
        </div>
      </section>

      {/* Depoimentos */}
      <section className="py-20 px-4">
        <h2 className="text-4xl font-bold text-center mb-12">O que nossos clientes dizem</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
          {[1, 2, 3].map((_, i) => (
            <Card key={i} className="bg-zinc-800 text-white border border-zinc-700">
              <CardContent className="p-6">
                <div className="flex items-center gap-2 mb-4 text-yellow-400">
                  {[...Array(5)].map((_, j) => (
                    <Star key={j} size={16} fill="currentColor" />
                  ))}
                </div>
                <p className="text-zinc-300 mb-4">
                  "Desde que começamos a usar este SaaS, nossa produtividade disparou. Interface limpa e muito intuitiva."
                </p>
                <p className="text-sm text-zinc-500">— Cliente Satisfeito #{i + 1}</p>
              </CardContent>
            </Card>
          ))}
        </div>
      </section>

      {/* CTA Final */}
      <section className="text-center py-20 px-6 bg-gradient-to-r from-blue-600 to-violet-700">
        <motion.h2 
          className="text-4xl font-bold mb-6"
          initial={{ opacity: 0, scale: 0.95 }} 
          whileInView={{ opacity: 1, scale: 1 }} 
          transition={{ duration: 0.6 }}
        >
          Pronto para revolucionar sua rotina?
        </motion.h2>
        <Button className="text-lg px-6 py-4 rounded-2xl shadow-xl bg-white text-blue-700 hover:bg-zinc-200">
          Crie sua conta gratuitamente
        </Button>
      </section>

      {/* Rodapé */}
      <footer className="text-zinc-400 text-sm py-8 px-6 text-center bg-zinc-950">
        © {new Date().getFullYear()} Seu SaaS. Todos os direitos reservados.
      </footer>
    </div>
  );
}
