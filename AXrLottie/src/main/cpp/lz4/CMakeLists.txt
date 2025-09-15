target_include_directories(rlottie
    PRIVATE
        "."
    )
# Use 16 KB ELF alignment to support devices with page size greater than 4 KB
target_link_options(rlottie PRIVATE "-Wl,-z,max-page-size=16384")
