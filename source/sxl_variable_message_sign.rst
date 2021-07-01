Signal Exchange List
====================

Object Types
------------

Grouped objects
^^^^^^^^^^^^^^^

.. figtable::
   :nofig:
   :label: Grouped objects
   :caption: Grouped objects
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.30\linewidth} p{0.50\linewidth}

   ============  =============
   ObjectType    Description
   ============  =============
   ============  =============
..

Single objects
^^^^^^^^^^^^^^

.. figtable::
   :nofig:
   :label: Single objects
   :caption: Single objects
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.30\linewidth} p{0.50\linewidth}

   =================  ================================
   ObjectType         Description
   =================  ================================
   VMS-skylt          VMS-skylt
   VMS-skylt display  VMS-skylt displayyta för budskap
   =================  ================================
..

Aggregated status
-----------------

.. figtable::
   :nofig:
   :label: Aggregated status
   :caption: Aggregated status
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.20\linewidth} p{0.18\linewidth} p{0.18\linewidth} p{0.15\linewidth}

   ============  ========  ====================  =================  =============
   ObjectType    Status    functionalPosition    functionalState    Description
   ============  ========  ====================  =================  =============
   ============  ========  ====================  =================  =============
..

.. figtable::
   :nofig:
   :label: State bits
   :caption: State bits
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.30\linewidth} p{0.45\linewidth}

   ==========================  =============  =========
   State- Bit nr (12345678)    Description    Comment
   ==========================  =============  =========
   ==========================  =============  =========
..

Alarms
------

.. figtable::
   :nofig:
   :label: Alarms
   :caption: Alarms
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.10\linewidth} p{0.45\linewidth} p{0.07\linewidth} p{0.07\linewidth}

   =================  =============  =====================================  ==========  ==========
   ObjectType         alarmCodeId    Description                              Priority  Category
   =================  =============  =====================================  ==========  ==========
   VMS-skylt          `A002`_        Internt fel                                     2  D
   VMS-skylt          `A004`_        För låg temperatur                              0  D
   VMS-skylt          `A005`_        För hög temperatur                              0  D
   VMS-skylt          `A006`_        Dörr öppen                                      2  D
   VMS-skylt          `A007`_        Fel på ljusgivare                               2  D
   VMS-skylt display  `A011`_        Fel på dioder, budskap läsbart                  3  D
   VMS-skylt display  `A012`_        Fel på dioder, budskap delvis läsbart           2  D
   VMS-skylt display  `A013`_        Fel på dioder, budskap ej läsbart               2  D
   =================  =============  =====================================  ==========  ==========
..

A002
^^^^^

Internt fel


A004
^^^^^

För låg temperatur


A005
^^^^^

För hög temperatur


A006
^^^^^

Dörr öppen


A007
^^^^^

Fel på ljusgivare


A011
^^^^^

Fel på dioder, budskap läsbart


A012
^^^^^

Fel på dioder, budskap delvis läsbart


A013
^^^^^

Fel på dioder, budskap ej läsbart


Status
------

.. raw:: latex

    \newpage


.. figtable::
   :nofig:
   :label: Status
   :caption: Status
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.24\linewidth} p{0.10\linewidth} p{0.55\linewidth}

   =================  ==============  ==================================
   ObjectType         statusCodeId    Description
   =================  ==============  ==================================
   VMS-skylt display  `S001`_         Nummer på bild som visas
   VMS-skylt display  `S002`_         Vägvisning som visas
   VMS-skylt          `S010`_         Skylten Avställd
   VMS-skylt          `S011`_         Skylten Lokal
   VMS-skylt          `S094`_         GPS-koordinater enligt SWEREF99TM.
   VMS-skylt          `S095`_         Version av komponent
   =================  ==============  ==================================
..

S001
^^^^^^^^

Nummer på bild som visas


.. figtable::
   :nofig:
   :label: S001
   :caption: S001
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   ======  =======  =======  ========================================================
   Name    Type     Value    Comment
   ======  =======  =======  ========================================================
   number  integer  [0-255]  Nummer på budskap. Om inget meddelande visas skickas "0"
   ======  =======  =======  ========================================================
..

S002
^^^^^^^^

Vägvisning som visas


.. figtable::
   :nofig:
   :label: S002
   :caption: S002
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   ======  ======  ========  ==================
   Name    Type    Value     Comment
   ======  ======  ========  ==================
   bitmap  base64  [bitmap]  Budskap som bitmap
   ======  ======  ========  ==================
..

S010
^^^^^^^^

Skylten Avställd


.. figtable::
   :nofig:
   :label: S010
   :caption: S010
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   =======  =======  =================  ====================
   Name     Type     Value              Comment
   =======  =======  =================  ====================
   Disable  boolean  -False |br| -True  Manöverläge Avställd
   =======  =======  =================  ====================
..

S011
^^^^^^^^

Skylten Lokal


.. figtable::
   :nofig:
   :label: S011
   :caption: S011
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   ======  =======  =================  =================
   Name    Type     Value              Comment
   ======  =======  =================  =================
   Local   boolean  -False |br| -True  Manöverläge Lokal
   ======  =======  =================  =================
..

S094
^^^^^^^^

GPS-koordinater enligt SWEREF99TM. |br| Decimaler anges med punkt (.)


.. figtable::
   :nofig:
   :label: S094
   :caption: S094
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   ======  ======  ===========  =============
   Name    Type    Value        Comment
   ======  ======  ===========  =============
   E       string  [koordinat]  Öst-koordinat
   N       string  [koordinat]  Norr-kordinat
   ======  ======  ===========  =============
..

S095
^^^^^^^^

Version av komponent


.. figtable::
   :nofig:
   :label: S095
   :caption: S095
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.15\linewidth} p{0.08\linewidth} p{0.13\linewidth} p{0.50\linewidth}

   ======  ======  =======  ====================
   Name    Type    Value    Comment
   ======  ======  =======  ====================
   status  string  [text]   Version av komponent
   ======  ======  =======  ====================
..

Commands
--------

.. figtable::
   :nofig:
   :label: Commands
   :caption: Commands
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.24\linewidth} p{0.15\linewidth} p{0.40\linewidth}

   =================  ===============  ==================================
   ObjectType         commandCodeId    Description
   =================  ===============  ==================================
   VMS-skylt display  `M101`_          Tänd vägvisning-nr
   VMS-skylt display  `M102`_          Skicka ner vägvisning till skylten
   VMS-skylt          `M110`_          Objektet avställd
   =================  ===============  ==================================
..

M101
^^^^^

Tänd vägvisning-nr


.. figtable::
   :nofig:
   :label: M101
   :caption: M101
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.14\linewidth} p{0.20\linewidth} p{0.07\linewidth} p{0.15\linewidth} p{0.30\linewidth}

   ========  ================  =======  =======  =========================================================================
   Name      Command           Type     Value    Comment
   ========  ================  =======  =======  =========================================================================
   bitmapnr  setActiveMessage  integer  [0-255]  Nummer på vägvisning |br| Om inget textmeddelande skall visas skickas "0"
   ========  ================  =======  =======  =========================================================================
..

M102
^^^^^

Skicka ner vägvisning till skylten


.. figtable::
   :nofig:
   :label: M102
   :caption: M102
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.14\linewidth} p{0.20\linewidth} p{0.07\linewidth} p{0.15\linewidth} p{0.30\linewidth}

   ========  ==========  =======  ========  =========================================================================
   Name      Command     Type     Value     Comment
   ========  ==========  =======  ========  =========================================================================
   bitmapnr  setMessage  integer  [1-255]   Nummer på vägvisning |br| Om inget textmeddelande skall visas skickas "0"
   bitmap    setMessage  base64   [bitmap]  Vägvisning som bitmap
   ========  ==========  =======  ========  =========================================================================
..

M110
^^^^^

Objektet avställd


.. figtable::
   :nofig:
   :label: M110
   :caption: M110
   :loc: H
   :spec: >{\raggedright\arraybackslash}p{0.14\linewidth} p{0.20\linewidth} p{0.07\linewidth} p{0.15\linewidth} p{0.30\linewidth}

   ======  ==========  =======  =======  ============
   Name    Command     Type     Value    Comment
   ======  ==========  =======  =======  ============
   status  setDisable  integer  [0-1]    1 = avställd
   ======  ==========  =======  =======  ============
..

.. |br| replace:: |br_html| |br_latex|

.. |br_html| raw:: html

   <br>

.. |br_latex| raw:: latex

   \newline

