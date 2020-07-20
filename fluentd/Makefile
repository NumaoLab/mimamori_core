REPO_NAME =
FLUENTD_DIR =
FLUENTD_CONF_BASE_URL = https://raw.githubusercontent.com/NumaoLab/mimamori_core/master/fluentd

initFluentdConf:
	@if [ ! -e /root/${REPO_NAME}/fluentd/fluent.conf ]; then \
		curl -L -o ${FLUENTD_DIR}/action_detection.conf ${FLUENTD_CONF_BASE_URL}/action_detection.conf ; \
		curl -L -o ${FLUENTD_DIR}/actions.conf ${FLUENTD_CONF_BASE_URL}/actions.conf ; \
		curl -L -o ${FLUENTD_DIR}/data_sender.conf ${FLUENTD_CONF_BASE_URL}/data_sender.conf ; \
		curl -L -o ${FLUENTD_DIR}/fluent.conf ${FLUENTD_CONF_BASE_URL}/fluent.conf ; \
		curl -L -o ${FLUENTD_DIR}/processings.conf ${FLUENTD_CONF_BASE_URL}/processings.conf ; \
		curl -L -o ${FLUENTD_DIR}/scenarios.conf ${FLUENTD_CONF_BASE_URL}/scenarios.conf ; \
		curl -L -o ${FLUENTD_DIR}/sensors.conf ${FLUENTD_CONF_BASE_URL}/sensors.conf ; \
		curl -L -o ${FLUENTD_DIR}/system.conf${FLUENTD_CONF_BASE_URL}/system.conf ; \
		curl -L -o ${FLUENTD_DIR}/system_copy.conf ${FLUENTD_CONF_BASE_URL}/system_copy.conf ; \
	else\
		echo "fluentd conf files have been touched";\
	fi