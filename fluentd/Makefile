REPO_NAME =
FLUENTD_CONF_BASE_URL = https://github.com/NumaoLab/mimamori_core/tree/master/fluentd

initFluentdConf:
	@if [ ! /root/${REPO_NAME}/fluentd/fluent.conf ]; then \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/action_detection.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/actions.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/data_sender.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/fluent.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/processings.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/scenarios.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/sensors.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/system.conf; \
		curl -L -O ${FLUENTD_CONF_BASE_URL}/system_copy.conf; \
	else\
		echo "node is already installed";\
	fi