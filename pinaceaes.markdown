---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Pinaceaes
---
<div class="container">
  <h2>Genus Selection (for Pinaceaes)</h2>
  <br />
  <div class="accordion accordion-flush" id="accordionPanelsStayOpenExample">
    <div class="accordion-item">
      <h2 class="accordion-header" id="panelsStayOpen-headingOne">
        <button class="accordion-button" type="button" data-bs-toggle="collapse"
          data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="true" aria-controls="panelsStayOpen-collapseOne">
          Abies Genus (fir)
        </button>
      </h2>
      <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse show"
        aria-labelledby="panelsStayOpen-headingOne">
        <div class="accordion-body">
          <!--For loop to display the contents of the _writers directory-->
          <div class="row">
            {% for posts in site.abies %}
            {% assign content = post.content | strip_newlines %}
            <div class="col-md-4 text-center" style="">
              <div class="card"
                style="display: flex; justify-content: center; padding:8px; min-height:100px; border: 0; margin:10px 4px; box-shadow: 0 0 10px 5px rgba(0,0,0,0.045)">
                {% if posts.content == blank  %}
                <h5 class="card-title">{{ post.title }}</h5>
                {% else %}
                <h5 class="card-title">
                  <a href="{{ posts.url }}">{{ posts.title   }}</a></h5>
                {% endif %}
                <h6 class="card-subtitle mb-2 text-muted">{{ posts.Firs  }}</h6>

              </div>
            </div>
            {% endfor %}
          </div>
        </div>
      </div>

    </div>



  </div>
  <br />

  **Justifications for the Treatment of Abies**

  Infra-Abies delineations follow the combined nuclear, plastid, and morphological study of Xiang et al. (2018).
  Section-level classifications follow more targeted studies.

  **Section Abies**

  The Eastern Mediterranean Complex:
  The taxa A. bornmuelleriana and A. equi-trojani are frequently considered to be synonymous with the latter as the
  accepted name, but there is evidence that they are distinct taxa. Handel-Mazzetti named them at the same time in 1925
  from distinct geographical regions; therefore my classification here treating A. equi-trojani as a subordinate taxon
  follows the genetic data in Hrivnak et al. (2017) establishing it as a recent offshoot of A. bornmuelleriana. Coode
  and
  Cullen (1965) also considered these taxa to be distinct, and at the species level.
  Hrivnak et al. (2017) also provide evidence that A. x olcayana (putative A. bornmuelleriana x A. equi-trojani) is not
  a
  hybrid, but a recent evolutionary offshoot within A. bornmuelleriana s.l., much like A. equi-trojani. I adopt this
  treatment here, since it is clearly a distinct regional/ecological form worthy of conservation.
  Hrivnak et al. (2017) establish a close relationship between the above taxa and A. nordmanniana. They are maintained
  at
  the species level here to capture their variation, but there appears to be an argument for including them as
  subordinate
  subspecies/varieties under A. nordmanniana.
  Hrivnak et al. (2017) provide strong supporting data for Abies cilicica and Abies cilicica ssp. isaurica. The latter
  is
  quite rare and of major conservation concern. It is in North America, but it would be cool to acquire new genetics.

  _The Balkans Complex:_

  The taxa Abies alba, Abies cephalonica, and their putative hybrid A. borisii-regis are present in the Balkans, the
  latter as a putative stabilized hybrid. Krajmerova et al. (2016) provides data indicating that A. borisii-regis is a
  product of recent introgression resulting from contact between these two species, and is not a monophyletic stabilized
  hybrid species but rather a variable and complex hybrid swarm. Bella et al. (2015) also provide data showing that A.
  borisii-regis is genetically intermediate. Needle volatiles share the same tendency: clustering by species with A.
  borisii-regis intermediate (Nikolic et al. 2021). Despite its variable nature and hybrid origin, I record the name as
  A.
  borisii-regis here since it generally behaves as a stabilized hybrid species.

  _The North African Complex:_

  A. pinsapo has been historically treated as having three varieties: the type in Spain, and var. marocana and tazaotana
  in Morocco. Two studies, Terrab et al. (2007) and Sanchez-Robles et al. (2014) provide evidence for distinct but
  limited
  differentiation of the varieties, with the Moroccan varieties distinct from the Spanish populations but poorly
  differentiated from one another. It appears that treating marocana as a subspecies and tazaotana as a variety under it
  is reasonable and capture the hierarchy of differentiation.
  Sanchez-Robles et al. (2014) provide some evidence for a close relationship between A. alba and A. numidica.

  **Section Balsamea**
  The hybrid (koreana x lasiocarpa) has two grex names listed above, but neither have been validly published.

  **Section Pseudopicea**
  _The A. delavayensis complex:_

  Trees and Shrubs Online note that A. fabri seem to fall within a broad morphological interpretation of A. delavayi,
  but
  that it has a suite of unique characters warranting species status.

  _The A. chensiensis complex:_

  A. chensiensis, A. ernestii, A. recurvata, and A. salouenensis are all distinct but closely related species; retaining
  this treatment as proposed by Trees and Shrubs Online appears to be the preferable approach to describing their
  variation. The reference upholding A. salouenensis at species rank is Debreczy & Rácz 2011, as is the one referencing
  the likely parentage of A. x chengii.
  The taxon formerly known as A. chensiensis ssp. yulongxueshanensis has been sunk into synonymy with A. salouenensis by
  Flora of China, but requires further study.
  The critically endangered A. beshanzuensis and A. ziyuanensis are distinct, but the latter may be a subspecies of the
  former.

  _The A. forrestii complex:_

  The taxon known as A. forrestii var. georgei appears best treated as a distinct species (TSO).
  </div>