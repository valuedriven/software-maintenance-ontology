# Ontologia para Processo de Manutenção de Software

## 📌 Visão Geral

Este repositório contém o projeto de uma ontologia desenvolvida para apoiar o processo de manutenção de software. O objetivo é estruturar, representar e padronizar conhecimentos relacionados às atividades, artefatos, atores e fluxos envolvidos na manutenção, promovendo interoperabilidade, análise e automação.

A ontologia aqui descrita pode ser aplicada em ambientes de suporte, engenharia de software, gestão de conhecimento e sistemas de acompanhamento de tarefas, especialmente o Redmine.

---

## 🎯 Objetivos

* Estruturar conceitos essenciais do processo de manutenção de software.
* Aumentar a padronização na coleta, registro e interpretação de informações.
* Facilitar análises, recomendações e automações baseadas em conhecimento.
* Servir como base para integração com sistemas de gestão de chamados.

---

## 📁 Estrutura do Repositório

```
├── docs/               # Documentação detalhada da ontologia
├── ontology/           # Arquivos OWL/RDF
├── examples/           # Exemplos de instâncias e consultas SPARQL
├── scripts/            # Scripts para validação ou transformação
└── README.md           # Documento atual
```

---

## 🧠 Componentes da Ontologia

A ontologia inclui classes e propriedades para representar:

### **📘 Classes Principais**

* **ChangeRequest** – Solicitações de mudança ou chamados.
* **Artifact** – Artefatos manipulados (código, documentos, requisitos).
* **Task** – Atividades executadas durante a manutenção.
* **Actor** – Pessoas ou papéis envolvidos.
* **MaintenanceType** – Tipos de manutenção (corretiva, evolutiva, perfectiva, adaptativa).
* **ImpactLevel** – Grau de impacto da mudança.
* **SystemModule** – Componentes do sistema afetados.

### **🔗 Propriedades Principais**

* `affectsArtifact`
* `executedBy`
* `hasImpactLevel`
* `belongsToModule`
* `derivesFromRequest`

---

## 🛠️ Tecnologias Utilizadas

* **OWL 2** para modelagem ontológica.
* **Protégé** para edição.
* **RDF/XML, Turtle** como formatos de serialização.
* **SHACL** para regras de validação (opcional).

---

## ▶️ Como Usar

### **Visualizar a Ontologia**

1. Instale o [Protégé](https://protege.stanford.edu/)
2. Abra o arquivo em `ontology/*.owl`
3. Navegue pelas classes, propriedades e restrições.

### **Integrar com seu Sistema**

Exemplos de integração podem ser encontrados na pasta `examples/`.

---

## 📜 Exemplos de Consultas SPARQL

```sparql
PREFIX ont: <http://example.com/ontology#>

SELECT ?task ?actor
WHERE {
  ?task a ont:Task ;
        ont:executedBy ?actor .
}
```

---

## 🙌 Contribuindo

Contribuições são bem-vindas!

1. Faça um fork do repositório.
2. Crie uma branch com a nova funcionalidade.
3. Envie um Pull Request descrevendo suas alterações.

Consulte o arquivo `CONTRIBUTING.md` (caso exista) para mais detalhes.

---

## 📄 Licença

Este projeto é disponibilizado sob a licença MIT. Veja o arquivo `LICENSE` para mais informações.

---

## 📬 Contato

Para dúvidas, sugestões ou contribuições acadêmicas:

* **Autor/Pesquisador:** *[Junilson]*
* **E-mail:** *[junilsonl@hotmail.com](mailto:junilsonl@hotmail.com)*
* **Instituição:** *[UFMG]*

---

Obrigado por utilizar ou contribuir para este projeto!
