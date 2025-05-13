import yaml

# Sample Python dictionary
data = {
    'name': 'Alice',
    'age': 25,
    'skills': ['Python', 'Automation', 'CI/CD'],
    'details': {
        'employed': True,
        'experience': 4
    }
}

# Write the dictionary to a YAML file
with open('output.yaml', 'w') as file:
    yaml.dump(data, file, default_flow_style=False, sort_keys=False)

# Convert dictionary to YAML string and print it
yaml_string = yaml.dump(data, default_flow_style=False, sort_keys=False)
print(yaml_string)
