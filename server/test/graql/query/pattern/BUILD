#
# GRAKN.AI - THE KNOWLEDGE GRAPH
# Copyright (C) 2018 Grakn Labs Ltd
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as
# published by the Free Software Foundation, either version 3 of the
# License, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Affero General Public License for more details.
#
# You should have received a copy of the GNU Affero General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.
#

load("//dependencies/tools/checkstyle:checkstyle.bzl", "checkstyle_test")

java_test(
    name = "pattern-impl-test",
    test_class = "grakn.core.graql.query.pattern.PatternTest",
    srcs = ["PatternTest.java"],
    deps = [
        "//dependencies/maven/artifacts/com/google/guava:guava",
        "//server"],
    size = "small"
)

checkstyle_test(
    name = "checkstyle",
    targets = [
        ":pattern-impl-test"
    ],
)