project(DaxLDAV2011 NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

set(images
  images/DaxDiagram.pdf
  images/DaxPipelineVsTraditionalPipeline.pdf
  images/SimplePipeline.pdf
  images/ParallelVisPipeline.pdf
  images/SingleElementFilter.pdf
  images/worklet.pdf
  images/many_worklets.pdf
  )

add_latex_document(DaxLDAV2011.tex
  BIBFILES DaxLDAV2011.bib
  IMAGES ${images}
  MANGLE_TARGET_NAMES
  )

add_latex_document(DaxLDAV2011Presentation.tex
  IMAGES ${images}
  MANGLE_TARGET_NAMES
  )
