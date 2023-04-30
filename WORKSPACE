load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_cuda",
    sha256 = "404efdc116e94a28c4191cb294c4c818c2b2c132f73f7970f9c9326db9e7117e",
    strip_prefix = "rules_cuda-1e9954093c7d789c628ddf052035f725249c122f",
    urls = ["https://github.com/bazel-contrib/rules_cuda/archive/1e9954093c7d789c628ddf052035f725249c122f.tar.gz"],
)

load("@rules_cuda//cuda:repositories.bzl", "register_detected_cuda_toolchains", "rules_cuda_dependencies")

rules_cuda_dependencies()

register_detected_cuda_toolchains()

# Bazel Skylib.
http_archive(
    name = "bazel_skylib",  # 2022-11-16T18:29:32Z
    sha256 = "a22290c26d29d3ecca286466f7f295ac6cbe32c0a9da3a91176a90e0725e3649",
    strip_prefix = "bazel-skylib-5bfcb1a684550626ce138fe0fe8f5f702b3764c3",
    urls = ["https://github.com/bazelbuild/bazel-skylib/archive/5bfcb1a684550626ce138fe0fe8f5f702b3764c3.zip"],
)



http_archive(
    name = "minhashcuda",
    #sha256 = "",
    strip_prefix = "minhashcuda-d057b0769ef983aa1315ca8d78be6b6f67b380ae",
    urls = ["https://github.com/src-d/minhashcuda/archive/d057b0769ef983aa1315ca8d78be6b6f67b380ae.tar.gz"],
    build_file ="@//thirdparty:minhashcuda.BUILD"
)

http_archive(
    name="nlohmann_json",
    #sha256 = "",
    strip_prefix = "json-6af826d0bdb55e4b69e3ad817576745335f243ca",
    urls = ["https://github.com/nlohmann/json/archive/6af826d0bdb55e4b69e3ad817576745335f243ca.zip"],
)


http_archive(
    name="tokme",
    #sha256 = "",
    strip_prefix = "tokme-41d6f49e2ac3bddd8116a0ff0c56b35f370a9fae",
    urls = ["https://github.com/koth/tokme/archive/41d6f49e2ac3bddd8116a0ff0c56b35f370a9fae.zip"],
)
