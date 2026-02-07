# Engenharia de Software II - Atividade 3 (Etapas 2 e 3)

## Auditoria DevOps e Implementação de CI/CD: ScrapeGraphAI

Este repositório contém a implementação prática de uma esteira de Integração Contínua (CI) realizada para a disciplina de **Engenharia de Software II (UFS)**. O projeto foca na automação de processos para a biblioteca **ScrapeGraphAI**, garantindo a integridade do ambiente e a evolução sustentável do código.

---

## 👥 Equipe e Divisão de Temas

| Integrante(s) | Matrícula | Responsabilidade na Apresentação |
| --- | --- | --- |
| **Rafael Gomes / Breno Silva** | 202300095730 / 202300038968 | Arquitetura do Workflow Automatizado |
| **José Gabriel R. G. de Almeida** | 202300095599 | O Fluxo de Dados: Linha de Montagem Virtual |
| **Pedro Joaquim / Mateus Barreto** | 202300038897 / 202300038879 | Decisão Estratégica: Estratégia C |
| **José Victor / Maria Eduarda** | 202300038799 / 202300038860 | O Impacto Humano e Técnico da Automação |
| **Cauan Teixeira Machado** | 202300038627 | Introdução e Coordenação do Repositório Fork |

---

## 🔗 Acesso Rápido

* **Repositório Fork:** [Engenharia_de_Software-II_Etapa-3](https://github.com/mateus-barreto-dev/Engenharia_de_Software-II_Etapa-3)
* **Evidência de Sucesso (Green Build):** [Visualizar Logs no GitHub Actions](https://github.com/mateus-barreto-dev/Engenharia_de_Software-II_Etapa-3/actions/runs/21724918250)

* **Link do video no YT** [Clique Aqui]()

---

## 🛠️ Implementação da CI (Etapa 2)

A equipe adotou a **Estratégia C (Pipeline de Contingência)**. Esta decisão foi baseada em limitações técnicas do projeto original, que exige chaves de API pagas e alto poder computacional para execução de LLMs, o que inviabilizaria o uso de runners gratuitos do GitHub.

### Arquitetura do Workflow

O pipeline foi configurado no arquivo `.github/workflows/quality_gate.yml` e segue as etapas:

* **Gatilho (Trigger):** Disparo automático em cada `push` ou `pull_request`.
* **Checkout:** O sistema baixa o código-fonte no ambiente de execução.
* **Setup:** Configuração de um ambiente isolado com **Python 3.10**.
* **Smoke Test:** Execução do script `ci_demo.py` para validar a carga de bibliotecas e lógica básica.

---

## 📈 Discussão Crítica (Etapa 3)

### Combate ao Software Decay

A automação implementada funciona como um **sistema imunológico**, detectando anomalias na integridade do ambiente antes que se tornem problemas de degradação silenciosa causados por mudanças em dependências externas.

### Onboarding e Segurança Psicológica

A existência de um feedback imediato e automatizado provê segurança aos novos desenvolvedores. Ao reduzir a incerteza sobre a integridade do código após alterações, o pipeline encoraja a colaboração e acelera a curva de aprendizado.

