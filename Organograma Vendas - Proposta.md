config:
look: handDrawn
theme: base
class:
hideEmptyMembersBox: true
themeVariables:
primaryColor: '#fdd0e6'
primaryTextColor: '#f11075'
primaryBorderColor: '#f11075'
lineColor: '#f11075'
clusterBkg: '#fdf3f8'
clusterBorder: '#fe95c3'
fontFamily: 'Helvetica'
classDiagram
direction BT

namespace CXN["Customer Experience"] {

class GER["Enoli (Gerente de CX)"]

namespace JD["Jornadas Digitais"] {
    class ANA["Ana Machado (Coordenadora)"]
    class BOTVEN["Bot de Vendas"] {
        + Fernanda Liz
    }
    class BOTPOS["Bot de Pós-Vendas"] {
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
        + João
    }
    class EST["Estagiários"] {
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

style GER fill:#f11075,color:#FFFFFF,stroke:#f11075
style ANA fill:#fe95c3,color:#333333,stroke:#f11075
style MALU fill:#fe95c3,color:#333333,stroke:#f11075
style BOTVEN fill:#FFFFFF,color:#f11075,stroke:#f11075
style BOTPOS fill:#FFFFFF,color:#f11075,stroke:#f11075
style WPP fill:#FFFFFF,color:#f11075,stroke:#f11075
style REV fill:#FFFFFF,color:#f11075,stroke:#f11075
style AFC fill:#FFFFFF,color:#f11075,stroke:#f11075
style PAR fill:#FFFFFF,color:#f11075,stroke:#f11075
style EST fill:#FFFFFF,color:#5A5A5A,stroke:#BFBFBF
