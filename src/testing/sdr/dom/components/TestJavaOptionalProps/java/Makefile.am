TestJavaOptionalProps_jar_CLASSPATH = $(CLASSPATH_SOFTPKG_DEP)$(OSSIE_HOME)/lib/CFInterfaces.jar:$(OSSIE_HOME)/lib/log4j-1.2.15.jar:$(OSSIE_HOME)/lib/ossie.jar

TestJavaOptionalProps.jar: $(TestJavaOptionalProps_jar_SOURCES)
	mkdir -p bin
	$(JAVAC) -cp $(OSSIE_CLASSPATH) -d bin $(TestJavaOptionalProps_jar_SOURCES)
	$(JAR) cf ./TestJavaOptionalProps.jar -C bin .

clean-local:
	rm -rf bin

distclean-local:
	rm -f config.*
	rm -rf autom4te.cache
	rm -f acinclude.m4
	rm -f aclocal.m4
	rm -f configure
	rm -f depcomp
	rm -f install-sh
	rm -f ltmain.sh
	rm -f Makefile.in
	rm -f missing
	rm -rf .deps

ossieName = TestJavaOptionalProps
bindir = $(prefix)/dom/components/TestJavaOptionalProps/java/
noinst_PROGRAMS = TestJavaOptionalProps.jar
TestJavaOptionalProps_jar_SOURCES := $(shell find ./src -name "*.java")

xmldir = $(prefix)/dom/components/TestJavaOptionalProps/

domdir = $(prefix)/dom/components/TestJavaOptionalProps/java/
