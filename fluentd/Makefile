REPO_NAME =
FLUENTD_DIR =
FLUENTD_CONF_BASE_URL = https://github.com/NumaoLab/mimamori_core/tree/master/fluentd

initFluentdConf:
	@if [ ! /root/${REPO_NAME}/fluentd/fluent.conf ]; then \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/action_detection.conf -o ${FLUENTD_DIR}/action_detection.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/actions.conf -o ${FLUENTD_DIR}/actions.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/data_sender.conf -o ${FLUENTD_DIR}/data_sender.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/fluent.conf -o ${FLUENTD_DIR}/fluent.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/processings.conf -o ${FLUENTD_DIR}/processings.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/scenarios.conf -o ${FLUENTD_DIR}/scenarios.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/sensors.conf -o ${FLUENTD_DIR}/sensors.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/system.conf -o ${FLUENTD_DIR}/system.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/system_copy.conf -o ${FLUENTD_DIR}/system_copy.conf; \
	else\
		echo "node is already installed";\
	fi