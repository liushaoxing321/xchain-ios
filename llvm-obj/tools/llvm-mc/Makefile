##===- tools/llvm-mc/Makefile ------------------------------*- Makefile -*-===##
# 
#                     The LLVM Compiler Infrastructure
#
# This file is distributed under the University of Illinois Open Source
# License. See LICENSE.TXT for details.
# 
##===----------------------------------------------------------------------===##

LEVEL = ../..
TOOLNAME = llvm-mc

# This tool has no plugins, optimize startup time.
TOOL_NO_EXPORTS = 1
NO_INSTALL = 1

# Include this here so we can get the configuration of the targets
# that have been configured for construction. We have to do this 
# early so we can set up LINK_COMPONENTS before including Makefile.rules
include $(LEVEL)/Makefile.config

LINK_COMPONENTS := $(TARGETS_TO_BUILD) MCParser MC support

include $(LLVM_SRC_ROOT)/Makefile.rules
