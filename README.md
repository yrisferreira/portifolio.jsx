import React from "react";

const projects = [
  { name: "Aratiri Tecnologias", description: "Desenvolvimento de uma plataforma de e-commerce integrada com Odoo.", link: "#" },
  { name: "Aura", description: "Desenvolvimento de uma plataforma de e-commerce integrada com Odoo.", link: "#" },
  { name: "Automação - Power Automate", description: "Desenvolvimento de um aplicativo de automação para empresas de serviços.", link: "#" },
  { name: "Automação - UiPath", description: "Desenvolvimento de uma plataforma de e-commerce integrada com Odoo.", link: "#" },
  { name: "Automação - Automation Anywhere", description: "Desenvolvimento de uma plataforma de e-commerce integrada com Odoo.", link: "#" },
  { name: "Grafana", description: "Desenvolvimento de uma plataforma de e-commerce integrada com Odoo.", link: "#" },
];

const Portfolio = () => {
  return (
    <div className="bg-gray-100 text-gray-900 min-h-screen">
      <header className="bg-blue-500 text-white text-center py-6">
        <h1 className="text-3xl font-bold">Yris Ferreira</h1>
      </header>

      <main className="container mx-auto p-6">
        <h2 className="text-xl font-semibold text-center mb-6">Meus Projetos</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          {projects.map((project, index) => (
            <div key={index} className="bg-white p-6 rounded-lg shadow-md text-center">
              <h3 className="text-lg font-semibold text-blue-500">{project.name}</h3>
              <p className="text-gray-600 my-4">{project.description}</p>
              <a href={project.link} className="bg-blue-500 text-white py-2 px-4 rounded-lg hover:bg-blue-700 transition">
                Ver Projeto
              </a>
            </div>
          ))}
        </div>
      </main>

      <footer className="bg-gray-900 text-white text-center py-6 mt-10">
        <p>Email: <a href="mailto:yris@ferisan.com.br" className="text-blue-400">yris@ferisan.com.br</a></p>
        <p>
          <a href="https://www.linkedin.com/in/yrisferreira" target="_blank" className="text-blue-400 mx-2">LinkedIn</a> |
          <a href="https://github.com/yrisferreira" target="_blank" className="text-blue-400 mx-2">GitHub</a>
        </p>
        <p>&copy; 2025 Yris Ferreira - Todos os direitos reservados.</p>
      </footer>
    </div>
  );
};

export default Portfolio;
