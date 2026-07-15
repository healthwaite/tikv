Tag `v8.5.6` fails:

```
$ cargo test --package tikv --lib
...
    config::tests::test_cdc
    config::tests::test_check_critical_cfg_with
    config::tests::test_endpoint_config
    config::tests::test_region_size_config
    config::tests::test_validate_tikv_config
    coprocessor::statistics::analyze::tests::test_row_reservoir_sample_collector
    import::raft_writer::test::test_inflight_max
    storage::config::tests::test_validate_engine_type_config
```

Our branch (`6f8176596f858f995f31530603a60180040c1129 (HEAD ->
v8.5.6-cad-rebase)`) fails:

```
$ cargo test --package tikv --lib
...
    config::tests::test_cdc
    config::tests::test_check_critical_cfg_with
    config::tests::test_endpoint_config
    config::tests::test_region_size_config
    config::tests::test_validate_tikv_config
    coprocessor::statistics::analyze::tests::test_row_bernoulli_sample_collector
    import::raft_writer::test::test_inflight_max
    storage::config::tests::test_validate_engine_type_config
```
