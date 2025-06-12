DEFAULT_ARGS = -i inventory/hosts.yml -i inventory/state.ini

# Set this to the empty strin, to disable diff mode (on by default)
ANSIBLE_DIFF ?= --diff

all-check:
	ansible-playbook $(ANSIBLE_ARGS) $(ANSIBLE_DIFF) $(DEFAULT_ARGS) --check site.yml

test:
	echo "No tests defined"
