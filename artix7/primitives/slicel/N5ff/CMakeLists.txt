add_file_target(FILE ntemplate.N5ff.model.xml SCANNER_TYPE xml)

add_file_target(FILE ntemplate.N5ff.sim.v SCANNER_TYPE verilog)

add_file_target(FILE ntemplate.N5ff.pb_type.xml SCANNER_TYPE xml)
n_template(NAME N5ff.model.xml PREFIXES a;b;c;d SRCS ntemplate.N5ff.model.xml)

n_template(
  NAME N5ff.pb_type.xml
  PREFIXES a;b;c;d
  SRCS ntemplate.N5ff.pb_type.xml
)

n_template(NAME N5ff.sim.v PREFIXES a;b;c;d SRCS ntemplate.N5ff.sim.v
  APPLY_VERILOG_IMAGE_GEN
  )
