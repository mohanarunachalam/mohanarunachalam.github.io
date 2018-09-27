---
published: false
---
## A New Post

  To support our hypothesis, it helps to take a quick tour of common types
  of human diseases.
  To start, Bacterial infections are cured by flushing out all the bacteria
  from the body. Viral infections are also cured by flushing viruses out of
  the body. The problem is dealing with "viral reservoirs" that store parts
  of the disease even after the main viral bodies have been flushed. A big
  problem in finding a cure to AIDS.

  As opposed to infectious diseases, cancer is (mostly) a disease caused by
  local mutations (this statement is an oversimplification. Cancer can be
  infectious, transmitted by cancerous cells or viruses). Cancer is "cured"
  by flushing all the cancer cells out by killing them. In practice,
  remission rates remain high since not all cancer cells are killed.

  Immuno disorders (allergies, rheumatoid arthritis) appear to have
  behavioral causes. Lack of exposure to "dirty" environments might have
  caused these diseases. Many, many diseases look to be caused by
  immunological disorders, including Alzheimer's and the link.

  Obesity has no real cure. Diet and exercise help, but there appears to be
  a high rate of recidivism. Some rising evidence that microbiomes (the
  community of bacteria which naturally live in human intestines) may play
  critical roles in such disorders.

  Genetic disorders result from small mutations to critical genes. Often,
  single proteins cease to function properly, causing issues. Such
  disorders could potentially be cured by the rising tide of new genetic
  treatment therapies.

  Now that we have completed a basic tour of diseases, we can consider a
  basic tour of methods to cure these diseases. GWAS studies sequence
  thousands of patients and healthy people, and use a statistical model to
  find genomic variants correlated with the disease outcome. GWAS studies
  work excellently when a small number of genetic variants are strongly
  linked to the disease in question (CITE), but is much less useful when a
  large number of variants are loosely linked to the disorder (as is the
  case for diseases such as autism) (CITE).

  The basic strategy is to create a cell culture, a set of diseased cells
  which grow well in culture (that is in a plate containing agar). For
  cancer, a number of cancer cells lines have been created, which are cells
  harvested from cancerous tumours. Examples of such cell lines include the
  infamous HeLa cells (CITE). The major weakness of the cell culture
  approach is that it is never easy to verify that a particular cell
  culture comes from the source we believe. Cross contamination of
  cell-lines is a major problem here (CITE). The advent of cheaper
  sequencing might enable better quality control, by allowing researchers
  to regularly sequence their cell cultures to verify that they match the
  reference baseline. 

  Another weakness of cell culture data is that it is never clear if the
  induced response is merely an artifact of the cell residing in an
  unnatural growth medium. Tissues have cells arranged in more complex
  hierarchical formations, which themselves allow for more elaborate
  control structures between the cells (CITE). A recent improvement in this
  space is the advent of organoid models which grow cultures of cells into
  three dimensions pseudo-organs. This provides the hope of more accurate
  models which capture more of the disease biology.

  Knockout studies use gene editing in mice to test whether introducing or
  removing a gene causes onset or cure to the disease. The main advantage
  to this strategy is that it enables researchers to create a "model
  organism". That is, genetically modify or breed or infect animals
  (typically rats or mice) so that they have a version of the disease in
  question. Apply proposed treatments to said animals until one works. Move
  forward with that treatment to tests with human patients.

  This approach has many strengths. Since human understanding of biology is
  quite weak, it allows for testing biology with biology. The downside is
  that it's not easy to make animal models for more complex diseases, such
  as neurodegenerative diseases or mental disorders.
 I propose that the path forward is to systematically augment the use of
  animal models with computational disease  models. The thesis is to create
  models of disease using all available data from GWAS studies, animal
  models of the disease, and from clinical data. The computational model of
  the disease would then be tested with a prospective compound, and the
  constructed model must be capable of predicting the induced response.
  This induced response can be experimentally tested in one of the physical
  data sources, and the data obtained can be used to refine the
  computational disease model. This active learning loop would allow for
  fine tuning of the disease models.

  In this proposal, there would be a computational model of a tumor, or say
  of a bone-breakage, or of the patient pain. Predictions of treatments
  would proceed by testing against the model, and by filtering predicted
  outcomes with human insight from doctors. The advantage of this approach
  is that it provides an intellectual framework with which to approach
  personal medicine.


  Model Organoid reference:
  http://www.medicalnewstoday.com/articles/311599.php

########Learning-centric disease modeling could equally well serve for achieving the dream of personalized medicine. President Obama's [precision medicine initiative];(https://www.whitehouse.gov/the-press-office/2015/01/30/fact-sheet-president-obama-s-precision-medicine-initiative) has drawn significant attention to the challenge of tailoring treatments to individual patients. A learning-centric paradigm could make it possible to learn sophisticated models of individual patients' diseases.

