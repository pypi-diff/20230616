# Comparing `tmp/piplexed-0.1.0.tar.gz` & `tmp/piplexed-0.1.1.tar.gz`

## Comparing `piplexed-0.1.0.tar` & `piplexed-0.1.1.tar`

### file list

```diff
@@ -1,170 +1,171 @@
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 piplexed-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 piplexed-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 piplexed-0.1.0/noxfile.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 piplexed-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/11d6b39f6cba4d2e
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/127dcb1ba30ddcf
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/15bfbf56b63a49bf
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/167eebdb4af7390f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/192e92ac001e26b7
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/19cbd95c9289a631
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/1dea4d5719cc1423
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/1ff57634e6a66dc8
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/203a8f5b186c8fc6
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/211b175a529e26f3
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/232e5ae29eb9bd1b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/23510605b7387c1c
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/23c37fe43f45ec7f
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2476d65861bf0f2
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/26507904b525d5f1
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/27c9f0c4fc1cf1f6
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/282d8acb342c6cff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/299042298a241fda
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2a0ff1af55d48ebf
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2b968adef921969b
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2c0db55d341b3398
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2cbabb595e03549e
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/2dad58abc4915448
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/307a0323f8d05e66
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/34790f3ca98f317
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/34a9be65026626bf
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/367a339600da65a0
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/38070a60ec6594cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3878eaa1768f73c8
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/393eb43f2ce95419
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3aec3af9b8b5924f
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3d42306f51c125a0
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3e0e64b59cbf106e
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3eac65615e1350e2
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3f643bf273ed11ab
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/3fb828415f2a03d6
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/401aa974df9e0a45
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/4051b1a380200f7c
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/407d2cce9190879c
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/4554d1711ee56092
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/45ccd89ebc0c59d7
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/4b80b697a68d0c60
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/4ea99b3479c7b1e8
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/4fac7cf1e73552f
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/5197ad08aa2fed35
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/5538e5f7b28cf77b
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/57ded2f33549ac7e
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/583ecf97e28a2f49
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/5856185c69bbe03e
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/5abe6dace1abc189
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/61089da3f7ca4a3a
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/611fbeabbc49d26d
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/64d6b17742ed6cdf
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/653b4810d388ad5a
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/65735d9d70d5db4f
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/66f832185fcbd746
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/67fdee94ede45094
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/6c05fc7bef66df38
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/6c7308feb2f9b73b
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/6ca387d2f4094b65
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/6e117833a2672af6
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/6f922263e14d05e
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/71ac704e4fc2ff22
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/71b87829a73fb1a1
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/74affa49747a8a21
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/74c73099c5b038b6
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/7b69c1411b560f89
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/8887c9ebc38494ed
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/8a3ece506521f4e1
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/8be40173c0c9f5f3
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/8cb120de9b834099
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/8ce1a407fa348ee5
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/916173f3c6c6d707
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/923811c2cdeb312
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/94f4c6cbaf03343a
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9598b5ba2e0d59e3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/96630d28b2133cc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/970c71d92e1cabaa
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/99474b02eb11aa78
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/99db5d19cb582c00
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9ae00f211925a43d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9af7ca1c5d1883b4
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9b94adb60e57847f
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9d180ca4bd4ae4b1
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/9f4a4ec61cae3e58
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a0fd9247bda9fe90
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a64aab24899f5820
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a6634478cfded9ac
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a777140b381d529d
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a799ea1e264ebaa5
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/a99985c563031f81
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/aa865f81381385eb
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/aaa13f99ace4224f
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/ad188f5543733777
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/af3130fb2dbe450
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/b1c5a9ba694254f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/b77a839b24c0006d
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/b9483bc764789c9d
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/bb3f40040f22916c
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/c1342de3877f4d70
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/c2b55c91ac09218
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/c3349279edebcda1
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/c64ad1d69417d147
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/c6c02b4f37dc02a4
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/cce4cde473e4b344
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/cd4b98847b0e1506
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/cd635c3813708cac
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/ce445a7ff4377cdb
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/d04e3898dd6fc9e5
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/d1cb6144ca464be2
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/d6af49cace7bf05f
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/dcec0320f2e49a66
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/de1a76ee3ca75440
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/e071f35d1e4e4ced
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/e0a084becbd671a1
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/e0e3248ead74d9a8
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/e6ec294a4f0f096c
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/e85ee58bec5f2762
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/ed038bbe4141c820
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/ed9302eb5acd0dfa
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f1eef82f96d524ab
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f32cc2318af14a1
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f4c128bdc020732b
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f5497fe2c7b5f2f5
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f5783e7b04de3393
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f79e0bfc0b05836a
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/f81a236198b7c900
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/fb42fa356f00f31f
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/fbdb09b18e88d0ec
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/fdc665141b6abc89
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 piplexed-0.1.0/.ruff_cache/content/fe242f770708cbb6
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/Future-development.md
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/How-piplexed-works.md
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/Release-notes.md
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/Why-piplexed.md
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/index.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/css/custom.css
--rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/img/piplexed-list-outdated-pre.PNG
--rw-r--r--   0        0        0    22413 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/img/piplexed-list-outdated.PNG
--rw-r--r--   0        0        0    15479 2020-02-02 00:00:00.000000 piplexed-0.1.0/docs/img/piplexed-list.PNG
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/all.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/docs.in
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/docs.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/linting.in
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/linting.txt
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/pyproject.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/tests.in
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 piplexed-0.1.0/requirements/tests.txt
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/__init__.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/_print_tree.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/cli.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/pipx_venvs.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/pypi_info.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 piplexed-0.1.0/src/piplexed/version.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 piplexed-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 piplexed-0.1.0/tests/test_pipx_venvs.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 piplexed-0.1.0/tests/test_print_tree.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 piplexed-0.1.0/tests/test_pypi_info.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 piplexed-0.1.0/tests/test_version.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 piplexed-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 piplexed-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 piplexed-0.1.0/README.md
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 piplexed-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 piplexed-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 piplexed-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 piplexed-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 piplexed-0.1.1/noxfile.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 piplexed-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/11d6b39f6cba4d2e
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/127dcb1ba30ddcf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/12e949cab0f29fe3
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/15bfbf56b63a49bf
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/167eebdb4af7390f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/192e92ac001e26b7
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/19cbd95c9289a631
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/1dea4d5719cc1423
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/1ff57634e6a66dc8
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/203a8f5b186c8fc6
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/211b175a529e26f3
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/232e5ae29eb9bd1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/23510605b7387c1c
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/23c37fe43f45ec7f
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2476d65861bf0f2
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/26507904b525d5f1
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/27c9f0c4fc1cf1f6
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/282d8acb342c6cff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/299042298a241fda
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2a0ff1af55d48ebf
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2b968adef921969b
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2c0db55d341b3398
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2cbabb595e03549e
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/2dad58abc4915448
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/307a0323f8d05e66
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/34790f3ca98f317
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/34a9be65026626bf
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/367a339600da65a0
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/38070a60ec6594cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3878eaa1768f73c8
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/393eb43f2ce95419
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3aec3af9b8b5924f
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3d42306f51c125a0
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3e0e64b59cbf106e
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3eac65615e1350e2
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3f643bf273ed11ab
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/3fb828415f2a03d6
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/401aa974df9e0a45
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/4051b1a380200f7c
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/407d2cce9190879c
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/4554d1711ee56092
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/45ccd89ebc0c59d7
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/4b80b697a68d0c60
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/4ea99b3479c7b1e8
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/4fac7cf1e73552f
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/5197ad08aa2fed35
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/5538e5f7b28cf77b
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/57ded2f33549ac7e
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/583ecf97e28a2f49
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/5856185c69bbe03e
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/5abe6dace1abc189
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/61089da3f7ca4a3a
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/611fbeabbc49d26d
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/64d6b17742ed6cdf
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/653b4810d388ad5a
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/65735d9d70d5db4f
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/66f832185fcbd746
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/67fdee94ede45094
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/6c05fc7bef66df38
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/6c7308feb2f9b73b
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/6ca387d2f4094b65
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/6e117833a2672af6
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/6f922263e14d05e
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/71ac704e4fc2ff22
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/71b87829a73fb1a1
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/74affa49747a8a21
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/74c73099c5b038b6
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/7b69c1411b560f89
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/8887c9ebc38494ed
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/8a3ece506521f4e1
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/8be40173c0c9f5f3
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/8cb120de9b834099
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/8ce1a407fa348ee5
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/916173f3c6c6d707
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/923811c2cdeb312
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/94f4c6cbaf03343a
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9598b5ba2e0d59e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/96630d28b2133cc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/970c71d92e1cabaa
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/99474b02eb11aa78
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/99db5d19cb582c00
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9ae00f211925a43d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9af7ca1c5d1883b4
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9b94adb60e57847f
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9d180ca4bd4ae4b1
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/9f4a4ec61cae3e58
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a0fd9247bda9fe90
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a64aab24899f5820
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a6634478cfded9ac
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a777140b381d529d
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a799ea1e264ebaa5
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/a99985c563031f81
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/aa865f81381385eb
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/aaa13f99ace4224f
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/ad188f5543733777
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/af3130fb2dbe450
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/b1c5a9ba694254f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/b77a839b24c0006d
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/b9483bc764789c9d
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/bb3f40040f22916c
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/c1342de3877f4d70
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/c2b55c91ac09218
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/c3349279edebcda1
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/c64ad1d69417d147
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/c6c02b4f37dc02a4
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/cce4cde473e4b344
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/cd4b98847b0e1506
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/cd635c3813708cac
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/ce445a7ff4377cdb
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/d04e3898dd6fc9e5
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/d1cb6144ca464be2
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/d6af49cace7bf05f
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/dcec0320f2e49a66
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/de1a76ee3ca75440
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/e071f35d1e4e4ced
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/e0a084becbd671a1
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/e0e3248ead74d9a8
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/e6ec294a4f0f096c
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/e85ee58bec5f2762
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/ed038bbe4141c820
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/ed9302eb5acd0dfa
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f1eef82f96d524ab
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f32cc2318af14a1
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f4c128bdc020732b
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f5497fe2c7b5f2f5
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f5783e7b04de3393
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f79e0bfc0b05836a
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/f81a236198b7c900
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/fb42fa356f00f31f
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/fbdb09b18e88d0ec
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/fdc665141b6abc89
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 piplexed-0.1.1/.ruff_cache/content/fe242f770708cbb6
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/Future-development.md
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/How-piplexed-works.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/Release-notes.md
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/Why-piplexed.md
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/index.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/css/custom.css
+-rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/img/piplexed-list-outdated-pre.PNG
+-rw-r--r--   0        0        0    22413 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/img/piplexed-list-outdated.PNG
+-rw-r--r--   0        0        0    15479 2020-02-02 00:00:00.000000 piplexed-0.1.1/docs/img/piplexed-list.PNG
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/all.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/docs.in
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/docs.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/linting.in
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/linting.txt
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/pyproject.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/tests.in
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 piplexed-0.1.1/requirements/tests.txt
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/__init__.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/_print_tree.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/cli.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/pipx_venvs.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/pypi_info.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 piplexed-0.1.1/src/piplexed/version.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 piplexed-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 piplexed-0.1.1/tests/test_pipx_venvs.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 piplexed-0.1.1/tests/test_print_tree.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 piplexed-0.1.1/tests/test_pypi_info.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 piplexed-0.1.1/tests/test_version.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 piplexed-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 piplexed-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 piplexed-0.1.1/README.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 piplexed-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 piplexed-0.1.1/PKG-INFO
```

### Comparing `piplexed-0.1.0/CHANGELOG.md` & `piplexed-0.1.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog
 
-## [0.1.0](https://github.com/aj-white/piplexed/tree/0.1.0) - 2023-06-12
+## [0.1.1](https://github.com/aj-white/piplexed/compare/v0.1.0...v0.1.1) - 2023-06-15
+
+### Fixed
+
+- Erroneous github repo link in `pyproject.toml`
+
+## [0.1.0](https://github.com/aj-white/piplexed/tag/v0.1.0) - 2023-06-12
 
 ### Fixed
 
 - Handle `NoSuchProjectError` by not sending non-pypi packages (locally installed wheels) to PyPI API.
 - Various linitng and mypy errors have been squashed.
```

### Comparing `piplexed-0.1.0/mkdocs.yml` & `piplexed-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/noxfile.py` & `piplexed-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.github/workflows/ci.yml` & `piplexed-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/15bfbf56b63a49bf` & `piplexed-0.1.1/.ruff_cache/content/15bfbf56b63a49bf`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/167eebdb4af7390f` & `piplexed-0.1.1/.ruff_cache/content/167eebdb4af7390f`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/232e5ae29eb9bd1b` & `piplexed-0.1.1/.ruff_cache/content/232e5ae29eb9bd1b`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/26507904b525d5f1` & `piplexed-0.1.1/.ruff_cache/content/26507904b525d5f1`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/282d8acb342c6cff` & `piplexed-0.1.1/.ruff_cache/content/282d8acb342c6cff`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/2a0ff1af55d48ebf` & `piplexed-0.1.1/.ruff_cache/content/2a0ff1af55d48ebf`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/2b968adef921969b` & `piplexed-0.1.1/.ruff_cache/content/2b968adef921969b`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/2c0db55d341b3398` & `piplexed-0.1.1/.ruff_cache/content/2c0db55d341b3398`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/34a9be65026626bf` & `piplexed-0.1.1/.ruff_cache/content/34a9be65026626bf`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/38070a60ec6594cc` & `piplexed-0.1.1/.ruff_cache/content/38070a60ec6594cc`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/3f643bf273ed11ab` & `piplexed-0.1.1/.ruff_cache/content/3f643bf273ed11ab`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/401aa974df9e0a45` & `piplexed-0.1.1/.ruff_cache/content/401aa974df9e0a45`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/4051b1a380200f7c` & `piplexed-0.1.1/.ruff_cache/content/4051b1a380200f7c`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/4554d1711ee56092` & `piplexed-0.1.1/.ruff_cache/content/4554d1711ee56092`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/45ccd89ebc0c59d7` & `piplexed-0.1.1/.ruff_cache/content/45ccd89ebc0c59d7`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/5197ad08aa2fed35` & `piplexed-0.1.1/.ruff_cache/content/5197ad08aa2fed35`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/5538e5f7b28cf77b` & `piplexed-0.1.1/.ruff_cache/content/5538e5f7b28cf77b`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/57ded2f33549ac7e` & `piplexed-0.1.1/.ruff_cache/content/57ded2f33549ac7e`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/583ecf97e28a2f49` & `piplexed-0.1.1/.ruff_cache/content/583ecf97e28a2f49`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/5856185c69bbe03e` & `piplexed-0.1.1/.ruff_cache/content/5856185c69bbe03e`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/5abe6dace1abc189` & `piplexed-0.1.1/.ruff_cache/content/5abe6dace1abc189`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/64d6b17742ed6cdf` & `piplexed-0.1.1/.ruff_cache/content/64d6b17742ed6cdf`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/6c05fc7bef66df38` & `piplexed-0.1.1/.ruff_cache/content/6c05fc7bef66df38`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/6c7308feb2f9b73b` & `piplexed-0.1.1/.ruff_cache/content/6c7308feb2f9b73b`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/6e117833a2672af6` & `piplexed-0.1.1/.ruff_cache/content/6e117833a2672af6`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/71ac704e4fc2ff22` & `piplexed-0.1.1/.ruff_cache/content/71ac704e4fc2ff22`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/71b87829a73fb1a1` & `piplexed-0.1.1/.ruff_cache/content/71b87829a73fb1a1`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/74affa49747a8a21` & `piplexed-0.1.1/.ruff_cache/content/74affa49747a8a21`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/7b69c1411b560f89` & `piplexed-0.1.1/.ruff_cache/content/7b69c1411b560f89`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/8a3ece506521f4e1` & `piplexed-0.1.1/.ruff_cache/content/8a3ece506521f4e1`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/8cb120de9b834099` & `piplexed-0.1.1/.ruff_cache/content/8cb120de9b834099`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/916173f3c6c6d707` & `piplexed-0.1.1/.ruff_cache/content/916173f3c6c6d707`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/923811c2cdeb312` & `piplexed-0.1.1/.ruff_cache/content/923811c2cdeb312`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/99474b02eb11aa78` & `piplexed-0.1.1/.ruff_cache/content/99474b02eb11aa78`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/99db5d19cb582c00` & `piplexed-0.1.1/.ruff_cache/content/99db5d19cb582c00`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/9ae00f211925a43d` & `piplexed-0.1.1/.ruff_cache/content/9ae00f211925a43d`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/9f4a4ec61cae3e58` & `piplexed-0.1.1/.ruff_cache/content/9f4a4ec61cae3e58`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/a0fd9247bda9fe90` & `piplexed-0.1.1/.ruff_cache/content/a0fd9247bda9fe90`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/a64aab24899f5820` & `piplexed-0.1.1/.ruff_cache/content/a64aab24899f5820`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/a6634478cfded9ac` & `piplexed-0.1.1/.ruff_cache/content/a6634478cfded9ac`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/a799ea1e264ebaa5` & `piplexed-0.1.1/.ruff_cache/content/a799ea1e264ebaa5`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/a99985c563031f81` & `piplexed-0.1.1/.ruff_cache/content/a99985c563031f81`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/aa865f81381385eb` & `piplexed-0.1.1/.ruff_cache/content/aa865f81381385eb`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/b9483bc764789c9d` & `piplexed-0.1.1/.ruff_cache/content/b9483bc764789c9d`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/c1342de3877f4d70` & `piplexed-0.1.1/.ruff_cache/content/c1342de3877f4d70`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/c2b55c91ac09218` & `piplexed-0.1.1/.ruff_cache/content/c2b55c91ac09218`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/cd635c3813708cac` & `piplexed-0.1.1/.ruff_cache/content/cd635c3813708cac`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/ce445a7ff4377cdb` & `piplexed-0.1.1/.ruff_cache/content/ce445a7ff4377cdb`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/d04e3898dd6fc9e5` & `piplexed-0.1.1/.ruff_cache/content/d04e3898dd6fc9e5`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/d1cb6144ca464be2` & `piplexed-0.1.1/.ruff_cache/content/d1cb6144ca464be2`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/d6af49cace7bf05f` & `piplexed-0.1.1/.ruff_cache/content/d6af49cace7bf05f`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/dcec0320f2e49a66` & `piplexed-0.1.1/.ruff_cache/content/dcec0320f2e49a66`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/e071f35d1e4e4ced` & `piplexed-0.1.1/.ruff_cache/content/e071f35d1e4e4ced`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/e0e3248ead74d9a8` & `piplexed-0.1.1/.ruff_cache/content/e0e3248ead74d9a8`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/e6ec294a4f0f096c` & `piplexed-0.1.1/.ruff_cache/content/e6ec294a4f0f096c`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/e85ee58bec5f2762` & `piplexed-0.1.1/.ruff_cache/content/e85ee58bec5f2762`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/ed9302eb5acd0dfa` & `piplexed-0.1.1/.ruff_cache/content/ed9302eb5acd0dfa`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/f1eef82f96d524ab` & `piplexed-0.1.1/.ruff_cache/content/f1eef82f96d524ab`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/f32cc2318af14a1` & `piplexed-0.1.1/.ruff_cache/content/f32cc2318af14a1`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/f5783e7b04de3393` & `piplexed-0.1.1/.ruff_cache/content/f5783e7b04de3393`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/f81a236198b7c900` & `piplexed-0.1.1/.ruff_cache/content/f81a236198b7c900`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.ruff_cache/content/fdc665141b6abc89` & `piplexed-0.1.1/.ruff_cache/content/fdc665141b6abc89`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/Future-development.md` & `piplexed-0.1.1/docs/Future-development.md`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/How-piplexed-works.md` & `piplexed-0.1.1/docs/How-piplexed-works.md`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/Why-piplexed.md` & `piplexed-0.1.1/docs/Why-piplexed.md`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/index.md` & `piplexed-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/img/piplexed-list-outdated-pre.PNG` & `piplexed-0.1.1/docs/img/piplexed-list-outdated-pre.PNG`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/img/piplexed-list-outdated.PNG` & `piplexed-0.1.1/docs/img/piplexed-list-outdated.PNG`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/docs/img/piplexed-list.PNG` & `piplexed-0.1.1/docs/img/piplexed-list.PNG`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/requirements/docs.txt` & `piplexed-0.1.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/requirements/linting.txt` & `piplexed-0.1.1/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/requirements/pyproject.txt` & `piplexed-0.1.1/requirements/pyproject.txt`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/requirements/tests.txt` & `piplexed-0.1.1/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/src/piplexed/_print_tree.py` & `piplexed-0.1.1/src/piplexed/_print_tree.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/src/piplexed/cli.py` & `piplexed-0.1.1/src/piplexed/cli.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/src/piplexed/pipx_venvs.py` & `piplexed-0.1.1/src/piplexed/pipx_venvs.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/src/piplexed/pypi_info.py` & `piplexed-0.1.1/src/piplexed/pypi_info.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/tests/test_pipx_venvs.py` & `piplexed-0.1.1/tests/test_pipx_venvs.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/tests/test_print_tree.py` & `piplexed-0.1.1/tests/test_print_tree.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/tests/test_pypi_info.py` & `piplexed-0.1.1/tests/test_pypi_info.py`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/.gitignore` & `piplexed-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/LICENSE.txt` & `piplexed-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/README.md` & `piplexed-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `piplexed-0.1.0/pyproject.toml` & `piplexed-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 dynamic = ["version"]
 
 [project.scripts]
 piplexed = "piplexed.cli:app"
 
 [project.urls]
 Documentation = "https://aj-white.github.io/piplexed/"
-Issues = "https://github.com/unknown/piplexed/issues"
-Source = "https://github.com/unknown/piplexed"
+Issues = "https://github.com/aj-white/piplexed/issues"
+Source = "https://github.com/aj-white/piplexed"
 
 [tool.hatch.version]
 path = "src/piplexed/version.py"
 
 [tool.black]
 target-version = ["py311"]
 line-length = 120
```

### Comparing `piplexed-0.1.0/PKG-INFO` & `piplexed-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: piplexed
-Version: 0.1.0
+Version: 0.1.1
 Summary: Find outdated python packages installed with pipx
 Project-URL: Documentation, https://aj-white.github.io/piplexed/
-Project-URL: Issues, https://github.com/unknown/piplexed/issues
-Project-URL: Source, https://github.com/unknown/piplexed
+Project-URL: Issues, https://github.com/aj-white/piplexed/issues
+Project-URL: Source, https://github.com/aj-white/piplexed
 Author-email: Andrew White <white-aj@outlook.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

