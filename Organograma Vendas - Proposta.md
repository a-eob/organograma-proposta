# Organograma de CX

> Estrutura da área de Customer Experience.

```mermaid
---
config:
  look: handDrawn
  theme: base
  themeVariables:
    primaryColor: '#fdd0e6'
    primaryTextColor: '#f11075'
    primaryBorderColor: '#f11075'
    lineColor: '#f11075'
    clusterBkg: '#fdf3f8'
    clusterBorder: '#fe95c3'
    fontFamily: 'Helvetica'
---
classDiagram
direction BT

namespace CXN["Customer Experience"] {

    class GER["Enoli (Gerente de CX)"]

    namespace JD["Jornadas Digitais"] {
        class ANA["Ana Machado (Coordenadora)"]
        class BOTVEN["Bot de Vendas"] {
            + Fernanda Liz
        }
        class BOTPOS["Bot de P&#126;os-Vendas"] {
            + Fernanda Liz
        }
    }

    namespace CV["Canais de Vendas"] {
        class MALU["Malu (Coordenadora)"]
        class WPP["WhatsApp e Promotores"] {
            + Ana Paola
            + Jaqueline
        }
        class REV["Revendedores"] {
            + Fausto
        }
        class AFC["Afiliados e Clubes de Ponto"] {
            + Malu
        }
        class PAR["Parcerias e Marketplace"] {
            + Jo&#126;ao
        }
        class EST["Estagiarios"] {
            + Junior
            + Zina
        }
    }
}

GER <-- ANA
GER <-- MALU
ANA <-- BOTVEN
ANA <-- BOTPOS
MALU <-- WPP
MALU <-- REV
MALU <-- AFC
MALU <-- PAR
MALU <-- EST
