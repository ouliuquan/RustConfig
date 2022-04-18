# RustConfig
Self use Rust Config

# Hierarchical structure  

Cargo allows local configuration for a particular package as well as global configuration. It looks for configuration files in the current directory and all parent directories. If, for example, Cargo were invoked in /projects/foo/bar/baz, then the following configuration files would be probed for and unified in this order:

/projects/foo/bar/baz/.cargo/config.toml  
/projects/foo/bar/.cargo/config.toml  
/projects/foo/.cargo/config.toml  
/projects/.cargo/config.toml  
/.cargo/config.toml  
$CARGO_HOME/config.toml which defaults to:  
Windows: %USERPROFILE%\.cargo\config.toml  
Unix: $HOME/.cargo/config.toml  