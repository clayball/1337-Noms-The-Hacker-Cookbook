## set up auth for travis

travis login --pro  --github-token abdce18e9e378e33e67ab8e1efd261fb9b95c54542
git config --local travis.slug
travis pubkey -r DEAD10C5/1337-Noms-The-Hacker-Cookbook 

Public key for DEAD10C5/1337-Noms-The-Hacker-Cookbook:

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCwa/WdulsScCsTrps6GCAG6YltZJ3iC4qacWGOAkLnJci2MkkbQw9nSzQsufDHCdaqGdgLL0hlq3LM3B7ZOugbaN8FaneddyT9RrUfqaVvcY4o/0swfR5VDztRFjrzzoOAIaFrDyXzCPk13reF34r/xLnSm0o+vaU4CVd1cy4wxBM+wcYE8Q2OZyd2SWo5mBcbpGs26RNRqPK3lLSUyJwrC6sGX0I18pi+mjWtxasgoUJduKPrXyKxXB39+ElUMy3DJ5vGYG07oTEo7yNa6K00U4JecEzUCCCQAN6Q7gB6gDaAlzz2otpNKYTlk1do3In7yJAgy1UEPX0m2kK3l1aP70P+arV20mdSLuUMSvouHaBgKI+Spq/OTsSigU2dBsAkabtyVtgVqk2+ZK5/zdJuHbyaTT4d6FcaWCRSpGuvOZh+Z+TvPh0uFKYN0yWKtDwGrYAx0Xq7oFdP05qnmeab4+TlmXiPTT78pYIefV14N0EtxvFcnRTQaPvQ6A4pbHYnGW+928I8ZO3pBaVMxJdGJryaRsgQiN/rLdPLCJ+9GC91SM1XuMbdrv22wmqDUx0eACdG2SdsUJlKH5DaGLDY7QigmsC7oTKcEnqupenduo9RknkI4lGokrr/sPQqvzqCRDP1voxn8LCdl+ms9LYcnVFQH87Vqp+qb8wAzCXc2w==

travis encrypt GH_TOKEN=abdce18e9e378e33e67ab8e1efd261fb9b95c5454f -r DEAD10C5/1337-Noms-The-Hacker-Cookbook
Please add the following to your .travis.yml file:

  secure: "fAfD7w+ZY8fT0qC2H5PC"

Pro Tip: You can add it automatically by running with --add.
