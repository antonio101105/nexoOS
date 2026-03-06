# De los Scripts de Construcción Escritos Por: Jim Gifford <lfs@jg555.com>
# Modificado Por: Joe Ciccone <jciccone@linuxfromscratch.org>
# Cambios adicionales: George Boudreau <georgeb@linuxfromscratch.org>
#                     Manuel Canales Esparcia
#                     Pierre Labastie

CONFIG_CONFIG_IN = Config.in
CONFIG = menu

all: menuconfig
	@$$(grep RUN_ME configuration 2>/dev/null | sed -e 's@RUN_ME=\"@@' -e 's@\"@@')

menuconfig:
	@if grep -E -q '(COMMIT="trunk"|COMMIT="multilib")' configuration; \
		then sed -i /COMMIT/d configuration; fi
	@cp -a configuration configuration.old 2>/dev/null || true
	@CONFIG_="" KCONFIG_CONFIG=configuration \
	    python3 $(CONFIG)/menuconfig.py $(CONFIG_CONFIG_IN)

# Limpieza

clean:
	rm -f configuration configuration.old error

.PHONY: all menuconfig clean
