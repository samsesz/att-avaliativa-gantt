# att-avaliativa-gantt

```mermaid
gantt
title TechConnect Solutions
dateFormat YYYY-MM-DD

section Preparação
Levantamento de requisitos :a1, 2025-01-01, 14d
Documentação funcional :a2, after a1, 10d
Protótipos de interface :a3, after a2, 14d

section Desenvolvimento
Configuração do ambiente :b1, after a3, 7d
Criação do banco de dados :b2, after b1, 7d
Módulo de login :b3, after b2, 14d
CRUD de empresas :b4, after b3, 21d
Upload de logotipo :b5, after b4, 14d
Relatórios PDF/Excel :b6, after b5, 14d
Painel administrativo :b7, after b6, 14d

section Entregas Crystal
Entrega 1 - Login :milestone, m1, 2025-01-21, 0d
Entrega 2 - CRUD Empresas :milestone, m2, 2025-02-11, 0d
Entrega 3 - Upload Logotipo :milestone, m3, 2025-02-25, 0d
Entrega 4 - Relatórios PDF/Excel :milestone, m4, 2025-03-11, 0d
Entrega 5 - Painel Administrativo :milestone, m5, 2025-03-25, 0d
Entrega Final - Sistema Implantado:milestone, m6, 2025-06-30, 0d

```

#Grafico crystal

```mermaid
graph TD
 E1["Levantamento de Requisitos - Semana 1 - E"]:::branco
 E2["Documentação Funcional - Semana 2 - E"]:::branco
 E3["Layout do Sistema - Semana 2 - C"]:::branco
 E4["Entrega 1 - Login - Semana 3 - E"]:::branco
 E5["Entrega 2 - CRUD - Semana 6 - C"]:::amarelo
 E6["Entrega 3 - Upload - Semana 8 - C"]:::laranja
 E7["Entrega 4 - Relatórios - Semana 10 - E"]:::laranja
 E8["Entrega 5 - Painel Admin - Semana 12 - D"]:::vermelho
 E9["Entrega Final - Sistema Completo - Semana 24 - V"]:::vermelho

 E1 --> E2 --> E3 --> E4 --> E5 --> E6 --> E7 --> E8 --> E9

%% Definições de estilo
classDef branco fill:#ffffff,stroke:#000,stroke-width:1px;
classDef amarelo fill:#FFD80D,stroke:#000,stroke-width:1px;
classDef laranja fill:#FFA233,stroke:#000,stroke-width:1px;
classDef vermelho fill:#E64C3C,stroke:#000,stroke-width:1px;
