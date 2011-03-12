project(DaxLDAV2011 NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

add_latex_document(DaxLDAV2011.tex
  BIBFILES DaxLDAV2011.bib
  )
